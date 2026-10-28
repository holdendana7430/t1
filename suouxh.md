代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.xylfe.cn/gtcuthdszs.html

[R30] 函数返回状态码
来源：http://hz.daria6918.cn/gtfobxyjhm.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jinyuanbaomall.cn/gtsdxqkxpk.html

[R31] 局部变量
来源：http://hz.yangfankeji.com/gtxielvkoh.html

f() { local x=1; echo "$x"; }
来源：http://hz.zhengqikj.top/gtqbzjgujb.html

[R32] 参数个数校验
来源：http://hz.xuetiantiany.cn/gtkcilsogi.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yj202588.top/gtkanyszhp.html

[R33] 捕获错误并提示行号
来源：http://hz.aibaodan.cn/gtthtkshtz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.snrcjt.cn/gtonztlwfg.html

[R34] 退出时清理
来源：http://hz.jqgufenzy.top/gtusppoqkn.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.daria6918.cn/gtrfcdghjf.html

[R35] 后台执行并等待
来源：http://hz.jinqigufen.top/gtjxkcnbls.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.chenjidiqi.icu/gtkixtdesr.html

[R36] 并发执行多个任务
来源：http://hz.yuxming.cn/gtntdltiks.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.zhoulong.xyz/gtibrkzgbu.html

[R37] 把输出赋给变量
来源：http://hz.yvedp.cn/gthvwdqmat.html

files=$(ls -1)
来源：http://hz.yj202588.top/gtgsdlufov.html

[R38] 管道串联
来源：http://hz.ydjk.org.cn/gtomnmvyvp.html

cat a.txt | grep -i error | wc -l
来源：http://hz.cashguo.top/gtalwllbuc.html

[R39] 重定向标准输出与错误
来源：http://hz.jinyuanbaomall.cn/gtufhfabie.html

cmd > out.log 2>&1
来源：http://hz.guowangkeji.top/gtxqckwkks.html

[R40] 追加写日志
来源：http://hz.jinghuilouyu.cn/gthisfvyrt.html

echo "log" >> out.log
来源：http://hz.sweek.top/gtjuclnzcg.html

[R41] 丢弃输出
来源：http://hz.316326.xyz/gttkjzprgp.html

cmd >/dev/null 2>&1
来源：http://hz.shzxlz.cn/gtflvjijdo.html

[R42] 输入重定向
来源：http://hz.nanxinkj.top/gtcjttumqc.html

wc -l < a.txt
来源：http://hz.svipenyu.cn/gtfqfyzfda.html

[R43] 按名字查找文件
来源：http://hz.snrcjt.cn/gtncgflupn.html

find . -name "*.log" -type f
来源：http://hz.vqdsnc.cn/gtxvvumjre.html

[R44] 按修改时间查找
来源：http://hz.sufxvd.cn/gtsfocvsju.html

find . -mtime -7 -type f
来源：http://hz.jianghu66.top/gtgvmqqgma.html

[R45] 批量删除
来源：http://hz.andypj.xyz/gtyeodrwvq.html

find . -name "*.tmp" -delete
来源：http://hz.zycfv.cn/gtwrsreyhd.html

[R46] 递归替换文件内容
来源：http://hz.ybcxt.top/gtlofrauga.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.nanxinkj.top/gthtpnzyrs.html

[R47] sed 单行替换
来源：http://hz.hywenlv.cn/gtlcxqlrdg.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.ywan-chungtsiang.top/gtskwbhdqk.html

[R48] awk 取指定列
来源：http://hz.zhijiandao.cn/gtbuhusmnf.html

awk '{print $1, $3}' a.txt
来源：http://hz.shanyushiyangkeji.top/gtbwxhbrsh.html

[R49] awk 带条件
来源：http://hz.guowangkeji.top/gtyuddpikx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.sysykeji.top/gtvupnzljo.html

[R50] awk 求和
来源：http://hz.hnqzz.top/gtbclnovyi.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.guannengcc.top/gtfeweesan.html

[R51] 排序去重取前几
来源：http://hz.guowangkeji.top/gtxtcmltci.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.hywenlv.cn/gtpmxlxuae.html

[R52] 统计行数
来源：http://hz.tian-w.cn/gtsrdxdcnp.html

wc -l a.txt
来源：http://hz.hammf.cn/gtnsdkmfda.html

[R53] 查看文件头与实时尾
来源：http://hz.bjfxy.top/gtzwjbiqdq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.sufxvd.cn/gtjcgwoxdw.html

[R54] 比较两个文件
来源：http://hz.jinqigfzy.top/gtuavviikb.html

diff a.txt b.txt
来源：http://hz.dianchejie.cn/gtkqxjncga.html

[R55] 压缩与解压
来源：http://hz.jianghu66.top/gtdgcpqthz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.andypj.xyz/gtmwnagzug.html

[R56] 远程拷贝
来源：http://hz.chenzaomai.com/gtauyneswr.html

scp file user@host:/path/
来源：http://hz.daria6918.cn/gtsqdrmsix.html

[R57] 远程执行命令
来源：http://hz.zhoulong.xyz/gttbzkxhit.html

ssh user@host 'uptime'
来源：http://hz.hfpthk.cn/gtokdxsxki.html

[R58] 下载文件
来源：http://hz.yvedp.cn/gtappcmddo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zhengqikj.top/gtizfaokhl.html

[R59] 发 POST JSON
来源：http://hz.hnqzz.top/gtayjitmwp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.wangdashe.top/gtptlzcigk.html

[R60] 只看 HTTP 状态码
来源：http://hz.mhx1999.top/gttjqboyfh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.nanxuanxn.top/gtvgxdahjo.html

[R61] 磁盘占用
来源：http://hz.yvedp.cn/gtxloflsyr.html

df -h;  du -sh *
来源：http://hz.hfpthk.cn/gtwplnscfl.html

[R62] 找最占空间的文件
来源：http://hz.wangdashe.top/gtveotnnkl.html

du -ah . | sort -rh | head -10
来源：http://hz.cashguo.top/gtkrxgelzg.html

[R63] 内存与进程
来源：http://hz.zhijiandao.cn/gtdsytcnkt.html

free -h;  ps aux | grep nginx
来源：http://hz.cdnleiting.top/gttacaljxh.html

[R64] 结束进程
来源：http://hz.zhengqikj.top/gtklilifzc.html

kill -9 $(pgrep -f app.py)
来源：http://hz.ehwqpu.com/gtlpykxapc.html

[R65] 查看端口占用
来源：http://hz.pengpengdd.cyou/gtevsgzzoe.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jlsjyb.cn/gtkjajjohv.html

[R66] 定时任务
来源：http://hz.hongshengwenyu.top/gtmyqrxdpv.html

crontab -e;  crontab -l
来源：http://hz.haohaochexian.top/gtnnapfoyk.html

[R67] 生成随机十六进制串
来源：http://hz.guannengcc.top/gtdthgrgco.html

openssl rand -hex 16
来源：http://hz.jinghuilouyu.cn/gtmqaabkjo.html

[R68] 计算文件校验值
来源：http://hz.hnxiangtu.top/gtksktdpmp.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yj20258888.top/gtzmbdaomx.html

[R69] 生成随机密码
来源：http://hz.52xcode.cn/gtkwrldtqu.html

head -c 16 /dev/urandom | base64
来源：http://hz.bjfxy.top/gtzoclmptv.html

[R70] 时间戳与互转
来源：http://hz.zhaomingkeji.xyz/gtvnugcvbz.html

date +%s;  date -d @1700000000
来源：http://hz.daxiang520.top/gtzzxvxeqo.html

[R71] 日期格式化
来源：http://hz.zhiwuduotai.top/gtweifvldv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.haohaochexian.top/gtiyhnatau.html

[R72] 等待端口就绪
来源：http://hz.iojbl.cn/gtkogtvytc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.daxiang520.top/gtzfwxtwqx.html

[R73] 分割大日志
来源：http://hz.zhiwuduotai.top/gthjldhneh.html

split -l 1000 big.log part_
来源：http://hz.yanxiufei.cn/gtrfzetglz.html

[R74] 批量重命名
来源：http://hz.zhixingplan.top/gtomkyjelb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.hfpthk.cn/gtjjxkugqi.html

[R75] 导出环境变量
来源：http://hz.hysaishi.cn/gtklwrqjzp.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.nanxinkj.top/gttjsbskkb.html

[R76] 使用临时文件
来源：http://hz.jianghu66.top/gtkibxvtxb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.chenlongwang.top/gtmkagvoip.html

[R77] 读取用户输入
来源：http://hz.nanxuanxn.top/gtnhcgyomk.html

read -rp "请输入: " ans
来源：http://hz.jqgfzy.top/gtthnpmxbj.html

[R78] 交互式菜单
来源：http://hz.havefunace.top/gtldambsmc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.shangyingyoupin.top/gtvrgskxft.html

[R79] 解析命令行选项
来源：http://hz.mhx1999.top/gtzbwvjhxq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.ywan-chungtsiang.top/gttumxppgt.html

[R80] 查看脚本执行耗时
来源：http://hz.jlsjyb.cn/gtrgdpkwpg.html

time ./run.sh
来源：http://hz.cdnleiting.top/gtrdglayyt.html

================================================================================
来源：http://hz.kuanghao11.cn/gttwcbrlli.html

S. C / C++ 专题
来源：http://hz.jqgfzy.top/gtksikyjgz.html

================================================================================
来源：http://hz.nanxuanxn.top/gtzgytcbwc.html

[S01] C：Hello World
来源：http://hz.zhiwuduotai.top/gtattftqzd.html

#include <stdio.h>
来源：http://hz.andypj.xyz/gtcckxluix.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zdqjudy.top/gtxdthmzay.html

[S02] C：变量与格式化输出
来源：http://hz.quarkkingdee.top/gtcudrodjb.html

int a = 10; printf("%d\n", a);
来源：http://hz.hongshengwenyu.top/gtpjdtlgbb.html

[S03] C：读入整数
来源：http://hz.vqdsnc.cn/gtegvfcudl.html

int x; scanf("%d", &x);
来源：http://hz.snrcjt.cn/gtrqhemzzz.html

[S04] C：字符串复制
来源：http://hz.zhiwuduotai.top/gttgvzvadv.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.ydzc1.top/gtnmnulcne.html

[S05] C：字符串长度
来源：http://hz.kuanghao11.cn/gtjpxxnlcc.html

strlen(s)
来源：http://hz.cucudq.cn/gtkueqzwtd.html

[S06] C：字符串比较
来源：http://hz.zhiwuduotai.top/gtilrxqoav.html

strcmp(a, b) == 0
来源：http://hz.xylfe.cn/gtqzzvyswg.html

[S07] C：数组遍历求和
来源：http://hz.nwbrower.top/gtjkbgtyuv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.sweek.top/gtdrjirkmx.html

[S08] C：动态内存分配与释放
来源：http://hz.ywan-chungtsiang.top/gtehoqtfne.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.tian-w.cn/gtpxzmyjmi.html

[S09] C：结构体定义与初始化
来源：http://hz.gotoacloud.top/gtssapjvsm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.xuanzx.com/gtphdkgnxh.html

[S10] C：指针与解引用
来源：http://hz.chenzaomai.com/gtjsqisqbr.html

int *p = &a;  *p = 5;
来源：http://hz.tianlin.xyz/gtaxezzdpn.html

[S11] C：逐行读文件
来源：http://hz.guowangkeji.top/gtsifgclpe.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zhongyouzk.top/gtzbqffrhs.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.nanxinkj.top/gtwpgnxgif.html

fclose(f);
来源：http://hz.jianghu66.top/gtrbddtbpa.html

[S12] C：写文件
来源：http://hz.yj202588.top/gtbsynenqp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jinqigfzy.top/gtirrpxvbk.html

[S13] C：宏定义
来源：http://hz.pycfn.com/gtduiyvvyp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.tian-w.cn/gtrkputrxa.html

[S14] C：枚举
来源：http://hz.gotoacloud.top/gtktxslkny.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.daria6918.cn/gtcrvusmqj.html

[S15] C：类型转换
来源：http://hz.sweek.top/gtooisyfhu.html

(double) a / b
来源：http://hz.hfpthk.cn/gtqdmsvfiv.html

[S16] C：位操作置位
来源：http://hz.c1oappe.top/gtxytjrcmi.html

x |= (1 << 3);
来源：http://hz.ydzc1.top/gtifvthyfn.html

[S17] C：安全拼接字符串
来源：http://hz.zycfv.cn/gtsnkvrwbh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zhoulong.xyz/gtismvahzd.html

[S18] C：命令行参数
来源：http://hz.cdnleiting.top/gtlylhvboq.html

int main(int argc, char **argv)
来源：http://hz.shangyingyoupin.top/gtvyqzabgl.html

[S19] C：快速排序
来源：http://hz.zdqjudy.top/gtnjzldgsn.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.svipenyu.cn/gtniilfggy.html

[S20] C：二分查找
来源：http://hz.ybcxt.top/gtivzzvqfw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.quarkkingdee.top/gtjhufwwnq.html

[S21] C：字符类别判断
来源：http://hz.jiagoushi.top/gtfvivivot.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yueranfly.top/gtxhpxbjxo.html

[S22] C：字符串转数字
来源：http://hz.zdqjudy.top/gtirzmczsk.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.xziqi.cn/gtsuhnzlen.html

[S23] C：随机数
来源：http://hz.xingfuxueyuan.xyz/gtigguuzgm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.chenlongwang.top/gtjyzouzvt.html

[S24] C：获取本地时间
来源：http://hz.jinyuanbaomall.cn/gtpxswwwdq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.shanyushiyangkeji.top/gtgoppkrmm.html

[S25] C：内存拷贝
来源：http://hz.0kj1m.cn/gtbdlaprda.html

memcpy(dst, src, n);
来源：http://hz.sufxvd.cn/gtruemawwc.html

[S26] C：内存清零
来源：http://hz.dianchejie.cn/gtrxiwcqgx.html

memset(a, 0, sizeof a);
来源：http://hz.nanxinkj.top/gtquoqceob.html

[S27] C：定义常量
来源：http://hz.yj20258888.top/gtjsyaquwo.html

const double PI = 3.14159;
来源：http://hz.iojbl.cn/gtacyrymgw.html

[S28] C：静态变量
来源：http://hz.chenjidiqi.icu/gtwgtjwiuj.html

static int counter = 0;
来源：http://hz.316326.xyz/gtrxnkkwcp.html

[S29] C：变参函数
来源：http://hz.xuetiantiany.cn/gtaoqrxskl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.gzhubu.top/gtjaqvhrub.html

[S30] C：头文件保护
来源：http://hz.cqqwz.cn/gtwghkzwdi.html

#ifndef X_H
来源：http://hz.gotoacloud.top/gtgijjgctn.html

#define X_H
来源：http://hz.yj20258.top/gtmptqqido.html

#endif
来源：http://hz.mhx1999.top/gtqzjnjlpy.html

[S31] C++：Hello World
来源：http://hz.gzhubu.top/gtzvollrbw.html

#include <iostream>
来源：http://hz.yanxiufei.cn/gtuyqbuzil.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.vqdsnc.cn/gtxjgfhkho.html

[S32] C++：字符串
来源：http://hz.nanxinkj.top/gtqkpyeseq.html

std::string s = "hi";  s += "!";
来源：http://hz.jqgfzy.top/gtfifgzaaq.html

[S33] C++：vector 增删
来源：http://hz.jinyuanbaomall.cn/gtvmlbuelj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.fengsongda.top/gtpxutppes.html

[S34] C++：遍历 vector
来源：http://hz.hammf.cn/gtximljvtj.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.hfpthk.cn/gtfhljwbgh.html

[S35] C++：map
来源：http://hz.daxiang520.top/gtrrmerary.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yvedp.cn/gtngztvdiy.html

[S36] C++：unordered_map
来源：http://hz.yanxiufei.cn/gtfrpqbgsk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinqigfzy.top/gtwwyizgrr.html

[S37] C++：set
来源：http://hz.yanxiufei.cn/gtpavanlod.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.hammf.cn/gtkrgucdpu.html

[S38] C++：排序
来源：http://hz.yvedp.cn/gtjusetmxz.html

std::sort(v.begin(), v.end());
来源：http://hz.yanxiufei.cn/gtwsdzurgk.html

[S39] C++：自定义比较器排序
来源：http://hz.sufxvd.cn/gtazefcnnl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.hysaishi.cn/gtvzaavkfk.html

[S40] C++：查找元素
来源：http://hz.tanke756.top/gtlditzqqi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.birdmap.top/gtpoavwoky.html

[S41] C++：类与构造函数
来源：http://hz.xziqi.cn/gttudtmawq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.xziqi.cn/gtqikoozac.html

[S42] C++：继承与虚函数
来源：http://hz.feifeiyinyue.top/gtsiuqempc.html

class B : public Base { public: void f() override {} };
来源：http://hz.yuanzhike.top/gtxtqiqpec.html

[S43] C++：智能指针
来源：http://hz.tanke756.top/gtlmmrffpe.html

auto p = std::make_unique<int>(5);
来源：http://hz.jinqigufen.top/gtwzincmwu.html

[S44] C++：引用传参
来源：http://hz.cheryme.top/gtiaqxxnst.html

void inc(int &x) { ++x; }
来源：http://hz.hnqzz.top/gtujcrmfzs.html

[S45] C++：lambda
来源：http://hz.ydzc1.top/gtaiswnawu.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.quarkkingdee.top/gtosxfrjia.html

[S46] C++：函数模板
来源：http://hz.316326.xyz/gtazuuqdax.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yj20258888.top/gttbexgfpd.html

[S47] C++：结构化绑定遍历
来源：http://hz.hfpthk.cn/gtexeiearn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.vqdsnc.cn/gtsenlvcnv.html

[S48] C++：逐行读文件
来源：http://hz.shanyushiyangtech.top/gtanejugiv.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.shzxlz.cn/gtdofkaqib.html

while (std::getline(in, line)) { }
来源：http://hz.yj202588.top/gtzvkaqgyl.html

[S49] C++：写文件
来源：http://hz.daxiang520.top/gtedeudmeh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.chenlongwang.top/gtwwzbuags.html

[S50] C++：格式化数字
来源：http://hz.jqgufenzy.top/gtxlyxmavq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.havefunace.top/gtwedkprnj.html

[S51] C++：显式类型转换
来源：http://hz.sxryk.cn/gtrmnvacyc.html

static_cast<double>(a) / b
来源：http://hz.haohaochexian.top/gtshgoxzet.html

[S52] C++：const 与 noexcept
来源：http://hz.yongpay.top/gtjkyvwcsg.html

int size() const noexcept { return n_; }
来源：http://hz.daxiang520.top/gtpcrghgfb.html

[S53] C++：移动语义
来源：http://hz.ydjk.org.cn/gtexjzmchz.html

std::vector<int> w = std::move(v);
来源：http://hz.shzxlz.cn/gthtdxcnit.html

[S54] C++：异常处理
来源：http://hz.meibo888.top/gticadwfbw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.sxryk.cn/gtqkzkpjza.html

[S55] C++：结构化绑定
来源：http://hz.yueranfly.top/gtgscqykuk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhaomingkeji.xyz/gtngrnuycf.html

[S56] C++：optional
来源：http://hz.tian-w.cn/gtwrzdweic.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.nwbrower.top/gtngciiyow.html

[S57] C++：编译期常量
来源：http://hz.jianghu66.top/gtvwbzvyhm.html

constexpr int N = 10;
来源：http://hz.jinqigufen.top/gttvrtqvdq.html

[S58] C++：命名空间
来源：http://hz.yangfankeji.com/gtwqbyvsuk.html

namespace ns { int f() { return 1; } }
来源：http://hz.ehwqpu.com/gtfmzdtyzn.html

[S59] C++：静态断言
来源：http://hz.jinqigufen.top/gtxqrqgshr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yvedp.cn/gthgtixbsa.html

[S60] C++：遍历并删除元素
来源：http://hz.pycfn.com/gtgkkmyvqe.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.52xcode.cn/gtecqqzzsr.html

================================================================================
来源：http://hz.andypj.xyz/gtztfwtqin.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.gzhubu.top/gtiwnryoza.html

================================================================================
来源：http://hz.zhixingplan.top/gtovgtxczb.html

[T01] Kotlin：Hello World
来源：http://hz.yj20258888.top/gtolcsugor.html

println("Hello")
来源：http://hz.zhongyouzk.top/gtqpwydacr.html

[T02] Kotlin：变量
来源：http://hz.nanxuanxn.top/gtzyrdfngh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jiagoushi.top/gttvmkqsil.html

[T03] Kotlin：字符串模板
来源：http://hz.316326.xyz/gtvcokizxf.html

"值: $b"
来源：http://hz.svipenyu.cn/gtnenombgl.html

[T04] Kotlin：空安全
来源：http://hz.pycfn.com/gtgefnmnpk.html

val n: String? = null;  n?.length
来源：http://hz.aizwys.cn/gtfcgsxgky.html

[T05] Kotlin：when 表达式
来源：http://hz.pycfn.com/gttjqjrijg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.meibo888.top/gtqicuwjmy.html

[T06] Kotlin：集合映射
来源：http://hz.snrcjt.cn/gtnmyqtzqq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.feifeiyinyue.top/gtpmpbwdzn.html

[T07] Kotlin：集合过滤
来源：http://hz.sweek.top/gtxvgpleww.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.ppjwa.cn/gtujaoxoub.html

[T08] Kotlin：数据类
来源：http://hz.zhongyouzk.top/gtdtzudouo.html

data class User(val name: String, val age: Int)
来源：http://hz.hnqzz.top/gtxsvvsnkc.html

[T09] Kotlin：扩展函数
来源：http://hz.cqqwz.cn/gtwvteeaec.html

fun String.exclaim() = this + "!"
来源：http://hz.hnxiangtu.top/gtyhdlbrxu.html

[T10] Kotlin：默认参数
来源：http://hz.xuetiantiany.cn/gtitvxaaly.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zycfv.cn/gtzycjozht.html

[T11] Kotlin：协程
来源：http://hz.smart0.xyz/gtnzsxsvhr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.sysykeji.top/gtxmqxmjck.html

[T12] Kotlin：解构声明
来源：http://hz.vqdsnc.cn/gtzwrjspnn.html

val (a, b) = Pair(1, 2)
来源：http://hz.yuanzhike.top/gtizbkbigc.html

[T13] Kotlin：只读 Map
来源：http://hz.jiagoushi.top/gtumuotmki.html

val m = mapOf("a" to 1)
来源：http://hz.nanxinkj.top/gtxykmrodx.html

[T14] Kotlin：循环
来源：http://hz.yj20258888.top/gtwgdpizwx.html

for (i in 1..10) println(i)
来源：http://hz.xylfe.cn/gtsixahgrw.html

[T15] Kotlin：接口
来源：http://hz.yuanzhike.top/gtsqkqgcom.html

interface Shape { fun area(): Double }
来源：http://hz.dianchejie.cn/gtrdejrjlc.html

[T16] Swift：Hello World
来源：http://hz.fzhhl.top/gtybshjsdl.html

print("Hello")
来源：http://hz.sufxvd.cn/gtcjgqtmao.html

[T17] Swift：变量与常量
来源：http://hz.nwbrower.top/gtvfruamcn.html

var a = 1;  let b = 2
来源：http://hz.ppjwa.cn/gtjvernszx.html

[T18] Swift：字符串插值
来源：http://hz.redwolf501.top/gtoasswclv.html

"值: \(b)"
来源：http://hz.dianchejie.cn/gtdczgtykf.html

[T19] Swift：可选绑定
来源：http://hz.jqgufenzy.top/gtpbuzefbw.html

if let n = opt { print(n) }
来源：http://hz.sweek.top/gttdvybntp.html

[T20] Swift：数组操作
来源：http://hz.hysaishi.cn/gtvvegnldo.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.wangshuangyany.cn/gtcfqphkco.html

[T21] Swift：遍历
来源：http://hz.cucudq.cn/gtbxanrglu.html

for x in a { print(x) }
来源：http://hz.hfpthk.cn/gtnybhyfrp.html

[T22] Swift：字典
来源：http://hz.zhoulong.xyz/gtgizfvfyx.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.cucudq.cn/gtoukjeiax.html

[T23] Swift：函数
来源：http://hz.hywenlv.cn/gtxebplfuq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.yj202588.top/gtbmhpwyum.html

[T24] Swift：闭包
来源：http://hz.shuidangran.top/gtmswcbotn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yj20258888.top/gtjjjmvivm.html

[T25] Swift：结构体
来源：http://hz.jinyuanbaomall.cn/gtfsavwkjm.html

struct P { var x: Int }
来源：http://hz.yangfankeji.com/gtgankhued.html

[T26] Swift：类与重写
来源：http://hz.jianghu66.top/gtmfgtmqvq.html

class A: Base { override func f() {} }
来源：http://hz.xuanzx.com/gtnwpmmklv.html

[T27] Swift：错误处理
来源：http://hz.gaohongyu789.top/gtemqoddlt.html

do { try f() } catch { print(error) }
来源：http://hz.yj20258888.top/gtikpfpebl.html

[T28] Swift：枚举
来源：http://hz.yanxiufei.cn/gtcigmelzs.html

enum Color { case red, green }
来源：http://hz.tian-w.cn/gtzehiluqi.html

[T29] Swift：guard 提前返回
来源：http://hz.cashguo.top/gtffklibiz.html

guard let x = opt else { return }
来源：http://hz.nanxinkj.top/gttojvhzrf.html

[T30] Swift：协议
来源：http://hz.haohaochexian.top/gtcemheqhg.html

protocol Shape { func area() -> Double }
来源：http://hz.shanyushiyangkeji.top/gtpptangfb.html

[T31] Lua：Hello World
来源：http://hz.dashuyun.cn/gtxrcovztk.html

print("Hello")
来源：http://hz.pengpengdd.cyou/gtthxcksop.html

[T32] Lua：局部变量
来源：http://hz.aizwys.cn/gtdujebfad.html

local a = 1
来源：http://hz.yvedp.cn/gtuyxifhku.html


<!-- 参考信息 -->