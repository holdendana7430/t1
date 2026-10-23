代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3zutbzfob.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3bhocxcvx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3kivinevf.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3wcyztmxz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3ahjbuobs.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3fypgsbfr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3zbvxhdep.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3zzhbhqlw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3ololbcxn.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3rkoaoyma.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3togggwad.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3pfdcwpow.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3acifujqr.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3jymiuwom.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3mfqhvcxv.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3kxnxgfde.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3uvylnqpa.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3hchjnilf.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3jpgepmdn.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3rzainsrd.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3qinpycyz.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3bijwbjvy.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3risbrlnd.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3nfsjvviw.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3owivnclb.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3kpaonxhz.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3krpgflfi.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3ergeczrj.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3mzkzyvya.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3bubjfnil.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3shuuzqqu.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3apaiadzr.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3rybuycxw.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3nxquiqoq.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rxxfnvbz.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3puebuzaf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3ssekfllg.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3zqwtgcim.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ygbdmgrc.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3nptbafeq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3isitbviy.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3hteyfjrj.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3xaginwqn.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3msdpexwu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3dzeeglbb.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3apsakumk.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3hfyatjoc.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3feyknzpy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3rjcojlmr.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3rjezbtmh.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3gvbcrwda.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3hznhlqte.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3wdawaxbs.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3jpurkjid.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3kxmojztx.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3prbkuiat.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3upanhrvg.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3npkxblfv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3ajvdoxca.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3tcpvgpqf.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3eijmdhbm.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3juguhzln.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3awjsnurm.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3jndnovhz.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3ayunirou.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3mglktymk.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3drxgooie.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3ugrstcnf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3gbupnoqn.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3gofovhkr.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3jkhikuhk.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3jtbwiwjq.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3iaogenut.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3nkqxador.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tbjxcxir.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3pkmlygjz.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3eabzyrei.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3ilprqmti.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3qqrecims.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3tzwlkutf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3hcdirkvc.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3eodvqguy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3wwiijtit.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3sfnsfstc.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3zhsrmxbw.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3vofnubwi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3ekscgepj.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3lwgepnui.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3mwccujbr.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3qkbqjpdq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3qilgzccm.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3vznhcbty.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3gkspwadh.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3qrqkvhfs.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3zmickfzt.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3npkjhbkg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3lsltbhdw.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3ahhbowri.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3ojihjxmh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sstxohlw.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3mcopbxsg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ukxglqsq.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3urenmgoo.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3eylwjnwq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3isuwjopk.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3rpmtitsb.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3uhjjmsib.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3gwxeuotz.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3euhxmjns.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3iixwipzh.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3rwkuydxc.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3vadmrsdl.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3aaujgbzj.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3wcajolpg.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3qvcytibf.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3ulqdmgzn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3vxaaxttb.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3fhdornhh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3whznfbnr.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3htrgdsls.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3lqijyaid.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3cqglfpmp.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3evxpwyhe.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3pvnicukm.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3tzglsheo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3vexdwpjl.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3mwfbwktg.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3vgmoybhj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3lvlmxiub.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3dwblvmag.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3qszlompy.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3wyfhahah.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3bszydtqs.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3vwpmmsnx.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3xctngslz.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3oobvcemj.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3chnmrhnp.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bugbshmw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3vokcfxup.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3uoofeqph.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3bgjbvdrt.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3wdavderq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3asvrxlij.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3jebaqlps.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3jvybrbyy.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3ioqreigl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3xozolibv.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3dqeecvif.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3txvgtsdh.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3nsgcopmx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3vslggqxn.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3solvdhsw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3ugurrehz.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3gjqllbrj.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3xgmjdwih.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3cmdnkimz.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3oyeqgrev.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3aduotfbx.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xndgaohe.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3lvooriqv.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3pzlsrobb.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3jmjenxpo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3iyucwzro.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3lqcknfas.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3dzxvsfnt.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3hlcmetml.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3foirixwg.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wvaultgk.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3zhcwgmby.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ntiksgrj.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3wwttqdlm.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3uzlihtoa.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3miflysps.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pgbdhgvv.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3wtnksjas.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3lcmhojjy.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ouytdwcy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ajmftmfz.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3xzbjcekb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3slurzemk.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3czkytwbq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3tdyijlkn.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3bmsceqtf.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3rhxtymdf.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3vnjjysas.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3udvmhtsp.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3bmshuill.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3ousvreqp.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3vdetyxaj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3brlpypwa.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3ejntneip.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3xpzgkkzf.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3tkabhpnk.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3qxgiebgn.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3aphgzguj.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ohqdmoxc.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3fpedbutc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3ykrernoq.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3kzvhvwlw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxfukuzd.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3umaijirr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3wlfvmirn.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3whkgruhm.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3ksvmswmz.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3lmelakjg.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3etyrbqlg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3bjchjvyu.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3dcvfhcng.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3shlgsezo.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3qjtswefc.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3dqqfgtms.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3brxfemwy.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3gsmbcffv.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3qspcrxjh.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3xjlrgjmq.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3ultegkin.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3qqgrvnyn.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3gwuipepe.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zpbpupyi.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3dwylxhzz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3zzxojdqq.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3syxmtzwl.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ruaidoqx.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3rxmrpfsf.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dopmwzxk.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3prksmmur.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3xbgtqoao.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3aazyzlor.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3xenrssfy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3osuopgsv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3evoaqqtm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oplolfky.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qqvknzay.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ukxqidxa.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3gfdyjqks.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3sfklzahb.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3zkhnsjpt.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3vbhgzgkh.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3srhbdwxn.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3axckcoef.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3wztaozlk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3oxqbhjlc.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3kibfinhn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fnqmhdav.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hffakmgn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3vrucbdji.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3rrrirweu.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3zunucckr.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3fcuezlzk.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3amqzthfn.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3oiqgjjjq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3momxwfde.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3gdzchnbz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3nznaryzm.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3vmzmxtuf.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3bibyjukn.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3tfuoaxso.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3rvvnofvc.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3agdmtvon.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3dcfcqpmk.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3tpkhbszn.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3hgcrdxsb.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vbpwhycv.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3tlglmyee.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3xvkxitlr.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3dlbdyvju.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3cjnovpjj.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3szqmmdhd.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3gagipfrz.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3lttpbdxd.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3eqyuoaht.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3rjzfcqtr.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3pkfjqikr.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3nylwkfzl.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3qmuthwsl.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3uqzjgvur.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3afnlwjzk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3viflvgeb.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3hbwihzyr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3puqsqdea.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3hpuchhyl.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3dgesaiwm.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3gkiwhowr.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3fmxwodph.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3hhfgnlwm.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3wpcodsfy.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3bhhpbkhe.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3jqunfyhy.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3xtljdcru.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3bfrdavvt.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3ccsjeqms.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3cfnytyps.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qtxoptsi.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3lhgwdzas.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3dtsbrhls.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3hjugrivt.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3yjrujtgg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3hxwdljja.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3sxovrwbw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3bwgdzvfh.html


<!-- 参考信息 -->