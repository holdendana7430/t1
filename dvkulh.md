代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2behcyitc.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2xdfnqmrr.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2itajimbq.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2uiobiheb.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2izqamvmr.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2xfrrihve.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2efvtuool.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2xouanule.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2ztatbnuh.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2mercpyxt.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2udqeoafb.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2jnhctkwn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2prvifysa.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2rgyfszhe.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2jcivfnbt.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2ooxjrhvw.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2hltokxbu.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2kksdgnlj.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2ibopsmls.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2cqjwriej.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2zaxvvmie.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2wrnhkmux.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2bdrxxjdb.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2nbcqhdqu.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ukosmrik.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2tvmyvgvm.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pkghtkwu.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2yniwbdvg.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2rgljtqca.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2hefsbpip.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2tcxkgpcf.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2jmxoswrh.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2slkojsrf.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2fjjzgynk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2ylbmydjf.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2dfbnthlt.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jcjvradg.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2ujzzuljx.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2zotqvxsn.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2wgfqrodj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2itgsbmii.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2omdbyzyi.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wvjmcbvd.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2wkuzdrqu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2kgpsctxv.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2wqfhazdh.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2hzjqsmnt.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2bvdhjvpn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2qcwlfhue.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ofbqssqp.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2asvsicxm.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2wliiitrs.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2myaerviq.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2zjqsahnh.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2geqouyod.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2fdwmqlrk.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2hhnaymbq.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2olxxgkwx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2kafxyzfr.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2mxausxyg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2dghjdizp.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2cpgbyqgw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2getjflpg.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2kajubxtc.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2shxkpqji.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2ekgemcca.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2cmvmzmlo.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2hcxxvhsm.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2ozqwbkco.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2ikszrtda.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2kgirlpum.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2ttmiiifp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2hubzdcpn.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2luajnhxf.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2ziyihxnc.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2pervhajf.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2gunxcaea.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2vhmwdfpm.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mvfhdjnm.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2igdoeabl.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2bjzwnmmn.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2ssrizeth.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2tiecreul.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2iwfgkwqe.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2cujfluvp.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2jqmfmjut.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2pznieruw.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2xlqohoyj.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2iikgsgsh.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2hsdhzjis.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2sdwodjly.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2thwdksiv.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2gyrmebwp.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2ltfifhio.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2rnyzqowr.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2sotuexxr.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2eivrhlej.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2jpntykft.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2rjffrsvc.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2fhjsbhtp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2mllsqwie.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2smyweunk.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2ywymaflp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bazzzpbq.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2lynrgqmq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ztwrrkdc.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dlwwqhki.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2laipjlmc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2clnlujvx.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2sdnkmyyr.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2bdmxepoz.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2wusojoel.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2zebcripw.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2dwcvbzqj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2nrukrzsd.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2hgncpiyg.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2zsdrdilg.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ncygksfw.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2skapkrnp.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2xclxorxc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2avkhorjt.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2hmqogwbz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2cexvgqhy.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2vyaedwkh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2vpuhwenr.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2zagvqqct.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2yxlzxxbo.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2anqduviz.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2dbkkuzld.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2oqinkcbn.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2afkkzcgh.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2bsnhnvdy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2oyqvdpxl.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2cndyasgp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2amjhhjva.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2lfggipwo.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2mzyeiuro.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2lkcoyudg.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2iichoexf.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2qigqqmkh.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2pqfwfjtg.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tipztkhm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2pgydrdgo.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2wqoixvax.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2dezadveo.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2eomqqmxm.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2thmycueq.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2tvrntmwa.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2anguapzt.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2krelmdho.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2zrzifszf.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2vmbgbuap.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2fbdntomo.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2cevfyaak.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2ismwxcit.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2gpwciifz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2newcycgh.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2nkvikvcv.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2wtskaeoq.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2drkfxseg.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2brckapcd.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2xencaorm.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2allabcut.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2xlssvwfu.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ntekqclp.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2okdjrjzb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2vxbdwbly.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2vjvnnohf.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2cyurkiwn.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2qwdqxjzx.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2zbovjves.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dhdrbqzp.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2pymnicmr.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2vqsarrpy.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2ouklbxjf.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2ailerhei.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2ubcoptft.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fiiqxtgz.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ohepzxpt.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2egjsazst.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2qmroctwg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2phpwbuwf.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2qovprfzb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2igcudpge.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2ujjnjjpk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tasxisbf.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2pgrnaqsn.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2pxtfncaa.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2pjbuvmld.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2aiasogji.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2qmtmfnsc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2usfffmmq.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2woqhsael.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2trwbiifk.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2turuvdbf.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2oloiiart.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2lugetken.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2uyjnufok.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2mxseihev.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2clordngk.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2oatbngzz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2mrdsvzze.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2woakfswy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddzagdnu.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fpqpbczb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozlmbmja.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2pgqqcupu.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2tpfhqjul.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2cconctba.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2thlttxqv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ygqnltvg.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2rkblxeix.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2riyzuhpu.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2chcvjcsq.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2nuzelccw.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2btgtxedg.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2kepmhhxw.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2pzzqbuko.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2zofdpwvp.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2onaivswm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2fujrrmhw.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2wkhieimu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2mizgchiy.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2pymovbuw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2nwdighjb.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2jafflcms.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2soicjivb.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2xjvwmayy.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kmvfbhth.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2wljmsfva.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2edrokwmb.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2twkkwfik.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2skcvnpzv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vupildci.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2bfqepewk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kyzaioio.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2sdeompkk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2citnjuts.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2bptpyjwl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2mucorsvp.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2nihiksus.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2uvhmjorv.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2urfyotuq.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2rmhqdfvi.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2bjjnvdfm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2okuxfvro.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2oyqpuovm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2iznaknga.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2irdlnedy.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2lmsqpodf.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2myujvqkp.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2phglzrfr.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2fxkifcii.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2dqhjbwtr.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2vchwxmho.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2bmrldbsa.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2pedlkztb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2ppopnakw.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2hzgjgcpr.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2osxzeuii.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2mjyvszet.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cvshrtak.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2mvdmzmaj.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2uuajdbbd.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2vwuekjcv.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2gzrfwhby.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2avyccxoa.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2rfbjobwc.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2oiolltih.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2nkyvkfzi.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2pvwrezep.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2olzyfkfn.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2kiwftuky.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2jhwltdst.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2ytozwidi.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2fmuxmtyg.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yoylsgad.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2ugxrrcbz.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2izdczjym.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2tkpwgjhj.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2rakvikhr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2pkkimvra.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2bvcqyjpw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2joslaypb.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2uzsbxmok.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2vrhorqfw.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2tvyaehit.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2jqqjaprj.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2hoyqasba.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2ytddmjuo.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2kvjqrqpk.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2fmfykbdo.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2vfywhtwg.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2absrgsgr.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2bjxtiqez.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2tlleihds.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nmcfotwk.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2xyiabkjt.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2igwqsgwl.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2emhuapvl.html


<!-- 参考信息 -->