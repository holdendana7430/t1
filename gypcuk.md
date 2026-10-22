代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2okwlglzm.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2rnalsmjs.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwayhsur.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2krfcmtuu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2xbhufsni.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2dvqoedra.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2zacgudky.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2jipsvtqq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2tjwquovu.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2dozbifsh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2znbfrmts.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2ubsvnkdx.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2pffiewyy.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2gtmxmyso.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2ivxsiuyh.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2pwkmecmo.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2kncgaoxf.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2nwpbzatd.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2dgghddst.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2ftbsrdjj.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2littapli.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2dzwpnbgl.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rouvtvap.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2frhdlixt.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2fmrdjwsw.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2bsxvfkeb.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2wudotnvg.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2ywmnxewi.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2zbbvlbco.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2qzvjidhe.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2svzbmjdp.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2yawtwvpq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uchlawbi.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2nhwikbyn.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2trwnbzek.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2vzusxrmo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2xhwcsawy.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2kkbrhifs.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2snljuduf.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2glbgxtqc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2rfjldzmd.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2vkcqyvur.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2ifvqtdft.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2dmfaizdg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2jiufuily.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2xotctlue.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vpglsemp.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2gdyxxybt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2tbhgdpok.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2cdnwnsxh.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2fnnbqbqm.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2dxjoioix.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2mkgnkneb.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2nuhgkfwn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2jxbqacuj.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2mxksvphp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2sawblhff.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2fdlgtrye.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2mcdoggsf.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2zciijndc.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2fxvlqcrn.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2fsiwtwwk.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2vhdgfgaf.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2sldfzdwg.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2tatrixvd.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2kqjqngkx.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2rkrmassz.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2xnmhobkp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2uleakune.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2wlvelqtz.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2gjrduhse.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2ajknwxdv.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2iqoqaetv.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2wrusopem.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2ujiizmrf.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2xqcktamo.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2jhnyjvpq.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2qxkokcke.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2dyoacvtd.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lqqkmrmq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2btqwmmig.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2lqamhwaf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2xzkncmbm.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2mtrcmogh.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2xkphqfqa.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2lcflvaii.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2kypatfne.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2itxjdwlp.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2nkpflhfm.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2bhxlsoec.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2bmrfkzra.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2aqrkaofx.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2rsnsebzf.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2dvggjcgh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2oipujhxr.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2vyfdvoba.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2ovonvcge.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2mrqxdisb.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2vilguuzi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wjiqcbbd.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2irotwufm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vwyftumk.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pejpqpyv.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2fcnhjhcg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2kofssavz.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2wmehbunh.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2quwgrrmv.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2nhpyhfxq.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2widpjctx.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2bxdxblfm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2acauetcg.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2cshyxywo.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2utmjcfug.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2fbknjuga.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2tqxosrpb.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2kdjpjlte.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2qjldnedl.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2zgufxopu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2xbdjorat.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2idgctiom.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2shcxeiuj.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2etjeztfv.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2rqtwqbod.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2kodkclnd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2qzltheqo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2junndioo.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2mqzntbcp.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2chazimey.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2tkgdsyyk.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2hkfbmsua.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2palqvimu.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2nisceasv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2zcigshdc.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2wrtodfqg.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2briwxrhf.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2iofkiiju.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2rmojroxn.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zlzcecox.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2nmbeszby.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2qfjnpzwe.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2eqkfqwot.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2penskcyn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2wdeptjlb.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2cogfcery.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2pkankygn.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2rwdckdts.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2bbwjrbee.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2xawtwiaf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2bmndkghb.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2lmjtzhwh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2vrzhbcnk.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2aqukvqju.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2dxxdzhwh.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2borkxton.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2ctjrqjqc.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2vxyzmmfw.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2uyofhicb.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2kasdppvi.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ptooupnp.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2udskzsrr.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2ecjynnam.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2mspgtpdz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2oyvvrknj.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2frzxkyxh.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2cnhmyeeh.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2naovmxpr.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2orjycfjh.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2havtqsaa.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2nvpfkwgl.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2fryqocwz.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2ufujdxon.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2tajipymh.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2xwrnfucl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2igzsemdp.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2fidkyfsq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2idvkwxxt.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2yuqcztdb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qnquykde.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2nogpggvd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qazlfcqt.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2ptlbygbu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2qgxzaque.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2ofgxrwkg.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ysoilkkn.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2yjjzyhww.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2ztdzmyfa.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2gmaktqgq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2ittbdqiz.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2rvmsryfr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2eluflasz.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2yyedacye.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2cwpduudx.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2nyyxnaub.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2qrrahdhh.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2eptojnbq.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2njociuhu.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2cihnwexe.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2elcocysz.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2lnxymcqb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lsmfyycn.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2spbaicgb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2zdfkxaax.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ylhuucdl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2wwtcrrfm.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2fktvtqfy.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2tckpxttt.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2uqaosivb.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2rqfwkqqv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ymffnpbo.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2nhzicswg.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2exlujrws.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2eagnnole.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2kdsaavag.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2lgmbzbcb.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2tdunupvc.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2auxyazuu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2jwlumoxt.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ekzikwze.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2dkazluho.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2orxeijhd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2icevrdsj.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2yoqdpdui.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2trkovedl.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2nomgcezy.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ijtuiftg.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2btrzrqwv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2nijgwmpr.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2jdcgugyb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2qvidruer.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tgcgdxxe.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2npnqnofi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yuqxzufr.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yskykbnd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2exwsfhhq.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2fvfifolt.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2mgkrjhrr.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2vtgjiapi.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2hrwdbyem.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2cieulaev.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2yzlantkw.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2krvyqlbd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2qrdjqcwv.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2tdwirhme.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qpuinoei.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2aylynabk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2jcttgeap.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2knugwanh.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2vdrygrir.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2lsdvwmiv.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2hnwaxkib.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2rwkzupeu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2tlmlepbn.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2zdcderor.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2svxibzvf.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2heydyehm.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sbiuwxaz.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2uftwfxok.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2lvevtuig.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2fhapsano.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2cpmxtmmw.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2bbkqzpci.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2yvyxmplu.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ctdvyeze.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2udrqtumz.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2gskdfarv.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2ieqjixzt.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2kxvuaosr.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2gzdgxovh.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2tsiaozmu.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2ppfxaore.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2hgrzixuf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2veiiwjsz.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vkrjxype.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2bcjfaimo.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2jccoydoy.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2ksdwrort.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2gvavyupj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2zzhcharz.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ogklhkio.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ktpvczdt.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2dhtgzcuq.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2kzinyjpa.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2tcdapjgo.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2qvsbcqrl.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2dorzmlvt.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2pvsyzpwv.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2mdazezpw.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2bkyimapb.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2qthjysnv.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2faxtaiti.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2bvpyuwca.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2awznfvkn.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jfujxbsu.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ftszwxrt.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2meqcxuuo.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2bniksibl.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2xejjzibr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2bnzldfrs.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2ilkydrub.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2baxfvodm.html


<!-- 参考信息 -->