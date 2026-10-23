代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lpwnrhhh.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3uqkbbsfh.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvukttzr.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3mffiqcdb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3wchdyekt.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3bfbvpfib.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3lxlfrdby.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3zuukonta.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3mlndntsl.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3oggwqztf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3bvdgoaeo.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3kvucytow.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3udavchde.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3qdofmliu.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3pzghkxbz.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3wjoafbhm.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3xtjmjcfd.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3okfgkklw.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3jmqtvqij.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3lxywguqi.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ncbczxxj.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3rzpmvhwd.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jkzxonmi.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3yeczgifs.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3bokzqzlt.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3lnyqfjzo.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3wihwgtba.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3vzammjaf.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3plaormqu.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3hwcemkao.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3tytkkiuz.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3kniplmch.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3gkbrujhs.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3nmefcjzy.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ltmhnzok.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3kfpoixxp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3fkwajztf.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3rznqhhxp.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3opvkvvgf.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3cafpvmqj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3xbwlkvua.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3dmiugmal.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3ndandyav.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3wewzbqqq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3ytsuwyum.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3isradigb.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3swfesoii.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3bevagvpk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3uggpuhlh.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3zpjdupvt.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3oispkwek.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3tbilruab.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3aefvfpnl.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3rvuskjwf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ctlrbokk.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3hktctlji.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3jcutmrud.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3yznkqubu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3ywrhehzy.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3jmavxmbs.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3piefzvtj.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3zmalzeag.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3jgeroyey.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3wiclsjno.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3iynfzqhl.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3bahaqois.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3imysoxbq.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3jwiawmyh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3hfxzjhwy.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ypbuslte.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3mmeaxjuz.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3urljatjr.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3fqgpxbsj.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3tcrgrqrn.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3discluvz.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3ohsasslt.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3nyrdfgfg.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3rtmhgkty.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3mkuxkgau.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3xdhijzrv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3lmztcgif.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3zvjgrpok.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3xhaurvpe.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3jfwphxsq.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3elmdkrxe.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3tbgadaxx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3ihmvrooa.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3uwmgqcbk.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3efhnkkon.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3mghzqzwu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3jfofbtwp.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3tbupstkg.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3svxqbbmm.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3brbjxbfn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3chdcthpa.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3urmpwzuh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3htardavg.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3klyqjpim.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3uyyjgipy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mggcyams.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3nmsaljwj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dlmcimep.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jcjdypof.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3pihaksia.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3nvdwvymx.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3sihxbals.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3nioaktmz.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3edvkbtqb.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3pvahctka.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3jdkcoefc.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3kqidilbr.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3qnbsydol.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ebxnlgod.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3zqieldio.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3gidjbynj.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3aulmnprl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3rntgpwad.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3mfacjnoa.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3lyscpaqw.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3vgvfgptr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3fgkpieac.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3cnouxahl.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3kxatoedy.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3pcvbvtgs.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3lwduefbk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3twlfsjzq.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3qmvbwmik.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3rgueonvl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3rpuxlxpi.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3cprmcbcv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3gjfxwnjh.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3tszhehbb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3oboaigou.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3swjwcjfh.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3jgykyglr.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3uujapywq.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3gjbnrhwb.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ydlpbzrr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3idhduneg.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3rdloahha.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3acsqzmke.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3zcxdczeq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ytabmcdc.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3pvaygmzd.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3jfacpdzf.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3imiaovth.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3knosrotv.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3gpcragyl.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3hmxwgpyk.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3mvosdyla.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ljotdlgj.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3bkeojdwg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3hyekozqa.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3csdnkskq.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3onlsuoao.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3niaqmkar.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3ipwnxdoq.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3qrkzdxqk.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3uuujrmkh.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3zwmeipio.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3ykmtzvgl.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3gdvkxaca.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3uowwiubt.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3bkrvgjbn.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3znhxufjf.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3pycubclh.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3ufyffjcq.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3iarcital.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3nppwytrc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3tpjqsxfo.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lfzjxxzi.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3kskgxtrw.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3vifrsuwp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qfvmlgnk.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3bqjhsptn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3fcrysqhd.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ixvjmpha.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3luvxrdtm.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3fgsankpg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zrtzlofd.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3spkcyocu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3cwqxtzjg.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3jzsdotjn.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3bbhbwiyx.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3tsfiemwm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3cngsqnpu.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3sfzfpggv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3hoywkaod.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3qtqroyzm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3jftdrjny.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3parrktha.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3dnmeuybj.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3meokuclu.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3rgkcnpte.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3qvmiqfxq.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3hdunchhb.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3cpkdeozc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3rndkmdgj.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3gppeedwv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xytioier.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qkfoubxp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3asbtfvsv.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3tdlzucqy.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3lbprfdvz.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3jatiziac.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3pcfvscki.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3cjxdkcpe.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3qlxuirxw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xdaiwcfr.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3aqvswasx.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3jgodbjhl.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3aiajyikm.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3sqkgbiop.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3qjrpvuwd.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3hymzifpl.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3zzfedqgh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3jpwmefjc.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3svcvxqyw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3ypryjyla.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3gsbszcme.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3nqlgdvxd.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3txtihsji.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bnpczxjp.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3liqtekcn.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zqxdsauw.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3rwsovbig.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3mzvdhfre.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3bjhhdwsi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3sscuegzz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3szkezjxx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3uvvqyqgm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cugoibov.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kkolzdxk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jouydbil.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3zmhhtjtt.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3twsoxwva.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3wmhnswps.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ullmklvs.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3miolwnfr.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3iazntdqy.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fqhpjdmo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3tpnzyrne.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3jokcfxbv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ioqvlagg.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3fmzsjwqf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3ckhcyafh.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3kjgaowol.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3anbtdbmi.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3pnsbktnt.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3bebbjury.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3jojhyyqv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3fykkjkgj.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3zhzrvrpm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3ncjkabda.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3ivafquqp.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vnznkjpg.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3rvmhkxgb.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3lzuhsgdn.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3ntjyrmxh.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3klbiwthp.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3twdkrfpo.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3jyynnkxn.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3coyelfvk.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3kxfbdgvr.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3skznnvmq.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3slpfmhow.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3fcohyhxi.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3hcglvxeu.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3ltizxjpg.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3smnzhmge.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3wmuphoww.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3cznhamuw.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3mpgiaxhw.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3hfcdavpk.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3labwnktd.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3kbrabpaf.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3hpixqumv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3fcvhwufj.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3dhdtwqgq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3sartrdab.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3negmpzqd.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3ismevpfl.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3ppluwqgz.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3lgrifhsl.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3sibeamhj.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3kzjfyfaj.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3bqughmiv.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3tkrzfbgx.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3ezwmsucx.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3bmcoatty.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3ceflrsou.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3vaqhgonx.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3onsfwybf.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zltdabbq.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3odwvkekp.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3fpcivzft.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3izotmrvp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3ejdoqrka.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3fpoqxqyc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3egdjwvvb.html


<!-- 参考信息 -->