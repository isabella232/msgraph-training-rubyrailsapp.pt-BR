<!-- markdownlint-disable MD002 MD041 -->

<span data-ttu-id="060dc-101">Neste exercício, você criará um novo registro de aplicativo Web do Azure AD usando o centro de administração do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="060dc-101">In this exercise, you will create a new Azure AD web application registration using the Azure Active Directory admin center.</span></span>

1. <span data-ttu-id="060dc-102">Abra um navegador e navegue até o [centro de administração do Azure Active Directory](https://aad.portal.azure.com).</span><span class="sxs-lookup"><span data-stu-id="060dc-102">Open a browser and navigate to the [Azure Active Directory admin center](https://aad.portal.azure.com).</span></span> <span data-ttu-id="060dc-103">Faça logon usando uma **conta pessoal** (também conhecida como Conta da Microsoft) ou **Conta Corporativa ou de Estudante**.</span><span class="sxs-lookup"><span data-stu-id="060dc-103">Login using a **personal account** (aka: Microsoft Account) or **Work or School Account**.</span></span>

1. <span data-ttu-id="060dc-104">Selecione **Azure Active Directory** na navegação à esquerda e, em seguida, selecione **registros de aplicativo** em **gerenciar**.</span><span class="sxs-lookup"><span data-stu-id="060dc-104">Select **Azure Active Directory** in the left-hand navigation, then select **App registrations** under **Manage**.</span></span>

    ![<span data-ttu-id="060dc-105">Uma captura de tela dos registros de aplicativo</span><span class="sxs-lookup"><span data-stu-id="060dc-105">A screenshot of the App registrations</span></span> ](./images/aad-portal-app-registrations.png)

1. <span data-ttu-id="060dc-106">Selecione **Novo registro**.</span><span class="sxs-lookup"><span data-stu-id="060dc-106">Select **New registration**.</span></span> <span data-ttu-id="060dc-107">Na página **Registrar um aplicativo**, defina os valores da seguinte forma.</span><span class="sxs-lookup"><span data-stu-id="060dc-107">On the **Register an application** page, set the values as follows.</span></span>

    - <span data-ttu-id="060dc-108">Defina **Nome** para `Ruby Graph Tutorial`.</span><span class="sxs-lookup"><span data-stu-id="060dc-108">Set **Name** to `Ruby Graph Tutorial`.</span></span>
    - <span data-ttu-id="060dc-109">Defina **Tipos de conta com suporte** para **Contas em qualquer diretório organizacional e contas pessoais da Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="060dc-109">Set **Supported account types** to **Accounts in any organizational directory and personal Microsoft accounts**.</span></span>
    - <span data-ttu-id="060dc-110">Em **URI de Redirecionamento**, defina o primeiro menu suspenso para `Web` e defina o valor como `http://localhost:3000/auth/microsoft_graph_auth/callback`.</span><span class="sxs-lookup"><span data-stu-id="060dc-110">Under **Redirect URI**, set the first drop-down to `Web` and set the value to `http://localhost:3000/auth/microsoft_graph_auth/callback`.</span></span>

    ![Uma captura de tela da página registrar um aplicativo](./images/aad-register-an-app.png)

1. <span data-ttu-id="060dc-112">Escolha **Registrar**.</span><span class="sxs-lookup"><span data-stu-id="060dc-112">Choose **Register**.</span></span> <span data-ttu-id="060dc-113">Na página **tutorial do gráfico Ruby** , copie o valor da **ID do aplicativo (cliente)** e salve-o, você precisará dele na próxima etapa.</span><span class="sxs-lookup"><span data-stu-id="060dc-113">On the **Ruby Graph Tutorial** page, copy the value of the **Application (client) ID** and save it, you will need it in the next step.</span></span>

    ![Uma captura de tela da ID do aplicativo do novo registro de aplicativo](./images/aad-application-id.png)

1. <span data-ttu-id="060dc-115">Selecione **Certificados e segredos** sob **Gerenciar**.</span><span class="sxs-lookup"><span data-stu-id="060dc-115">Select **Certificates & secrets** under **Manage**.</span></span> <span data-ttu-id="060dc-116">Selecione o botão **Novo segredo do cliente**.</span><span class="sxs-lookup"><span data-stu-id="060dc-116">Select the **New client secret** button.</span></span> <span data-ttu-id="060dc-117">Insira um valor em **Descrição**, selecione uma das opções para **Expira** e escolha **Adicionar**.</span><span class="sxs-lookup"><span data-stu-id="060dc-117">Enter a value in **Description** and select one of the options for **Expires** and choose **Add**.</span></span>

    ![Uma captura de tela da caixa de diálogo Adicionar um segredo do cliente](./images/aad-new-client-secret.png)

1. <span data-ttu-id="060dc-119">Copie o valor secreto do cliente antes de sair desta página.</span><span class="sxs-lookup"><span data-stu-id="060dc-119">Copy the client secret value before you leave this page.</span></span> <span data-ttu-id="060dc-120">Você precisará dele na próxima etapa.</span><span class="sxs-lookup"><span data-stu-id="060dc-120">You will need it in the next step.</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="060dc-121">Este segredo do cliente nunca é mostrado novamente, portanto, copie-o agora.</span><span class="sxs-lookup"><span data-stu-id="060dc-121">This client secret is never shown again, so make sure you copy it now.</span></span>

    ![Uma captura de tela do novo segredo do cliente recentemente adicionado](./images/aad-copy-client-secret.png)