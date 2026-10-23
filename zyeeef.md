代发 wailian999

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3oqiuzfwy.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3cwtkesdh.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3xvflauuv.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3bnfveyfs.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3olvgecaq.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3drziwgak.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3uurvcfij.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3hixyzwbh.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wjadqzue.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3ooljepbq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3yhjgnaec.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3iufzseer.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3rytvefyv.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3wjzwpsbq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3kvnzpizm.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ofroxqhq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3golxvtwv.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3oqasuppx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3uxcpmmzo.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3pnkcsfjw.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3vlqmywwx.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3kmrkzmsn.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3ypxhhtxa.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3jzkmugoe.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3mtyfhjyw.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3akfgjkaa.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3kwjgpwxa.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3jywzzasx.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3xbznusdh.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3wusmrjgk.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fvjtsgil.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3rkeuxldm.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3vsveavmw.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3hhyuxjik.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3oiwhmfex.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3ekxjnvbr.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3aciwfxqc.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3byqkyaxv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3dqgbqhba.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3trktbycp.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3gaxxvwvt.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3tepyufkx.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jvuzuavj.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3qwvneukm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3dtwehzso.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3rrzvvmoo.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3dlhqbusw.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3nzzeslck.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3lnloigdo.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3vgqduyxx.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gpgsxzml.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3dkjszleb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3pfjhsxan.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3rlfbiivj.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bwqxkqvl.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3pcasjpgi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3rcicrczf.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3lcxzmghs.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3ztmcxalg.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3avjsezmy.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3ztogztpc.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3iayeparf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3qwdmukna.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3petxsrtb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3ufnagvgk.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3vhdumnnm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3zhudkxte.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3hegvekcd.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3hemkaphx.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3ksohaxrx.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3qniqhfqp.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3phiuphoa.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3xamxhxhy.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3fczcwwfs.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3utkvtwwd.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3vquhdfix.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3ibdlgzqo.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3nblgoxpo.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3npvuiztb.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3zqxewfzb.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3jmggbthc.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3zqzvahdc.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rikagcjq.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3wbdisyoy.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3rnovaluw.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3kmbqtqqr.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3zuuafaen.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ckdrtknu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3lyonlmhr.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3lfpzyzqh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3gjqgzxbf.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3bzdzcptn.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3gwvnrcdv.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3qbcbwghq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3whfbfvxf.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3psoydxzl.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3caowykpe.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3rameqyhv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3bdkzxtkc.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3hgtgezvz.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3swjvtvtc.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3ppkrzwvb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3gwrvxksk.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3iagqpaed.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3dtawsdgd.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3qnxhjlnc.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3dkmbbttt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vtxaaqux.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3gwhepiwf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zphjckwp.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jjujkzcc.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3qpchqosk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybmosuki.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3yudyyvug.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3lcsxpyfq.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3emsvjmeo.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3bcrxmdad.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3ecopmidv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3lasumatp.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3mnpjcdde.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3okaetsie.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3rlqbjewe.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3ynfgtwwh.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3tugggkvf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3mgkqqqlq.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3hoywhjhw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3gfsjkzpq.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3huqvzseg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3iocwgudv.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3cxivlibv.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3tezifwhy.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3nrovshfu.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3ogtxugkx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3anvbczhr.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3jgfyniwf.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3psjmubef.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3faegrftg.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3iimmgwme.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3unvfpsan.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ejjyzjuy.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3drdemofe.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3fhpjuytx.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3ooqgihwj.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3vzvmgghy.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3nqaelvnb.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ycmldpaj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3aouwvtcx.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3afgyffww.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3tpkcthvd.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3jkyvirys.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3nkgfeedc.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3ojzycfxz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3cunimnqw.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3ebuzayjl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3skaqcppi.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3rzcnlfct.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3ztcddeth.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3zbmbjurt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3ycfgwsor.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3wwkqumyo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3zksvlbnc.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ukuvclqy.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3azymtdrr.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3qmmvjpat.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3xljcjlsr.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3eypstizl.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xdczjoyj.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3flckeoez.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3yfymyotb.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3qlvbsnwk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3zxscclfn.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3ixqntqgn.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3daqhuqxn.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3flflmjff.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3uwloyiau.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3amxzmtry.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3rwekjsrh.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3tyjewzfc.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yurlsdbs.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3fnfhoiuj.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3pgzrsggc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3xjaacdqz.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3zezsflnk.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3vuyydimq.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3hdculaci.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3umsuqdix.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3yctpnbao.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3omprhdkx.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3ajcgexyv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3ywhodzae.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3hhedaqcg.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ozadiaby.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3hglektup.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3rujsmdgz.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3xwtzwmuv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3moahgpaw.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3qbxjafwb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3mamoflbx.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3foyphkcd.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3ijcxbyux.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ygkbdqzq.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3wemnayuj.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3ggclhnyp.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3ztqognuh.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3ugzkqlih.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3jzwpsqii.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3jredenmv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lykyikwx.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3czhndjst.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3gologjii.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rcrspecn.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3mkqqavdv.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3htvtbvcv.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3ifcjygam.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3vhrtvqcb.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3xepumyhy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ymriyeai.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3phheozma.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3ytfwsgdk.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3rwozylpw.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3wglyxdje.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3aljarpgw.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3rmupacoo.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3ixllxzkk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3dhlahbpv.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3jpqbcbwj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ldimftzd.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3fyhrjlik.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3edutipxc.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3xbeorrlh.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3hfunufzo.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3saoszklg.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rjvyuacs.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3kyudczdy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3usrqjbsb.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3itpwngmc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3rcwequnv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kgwdbfsm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3rjrwbhba.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3weajsypt.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3etrbggvo.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3rdhqtiqn.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3kwmwqnbt.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3bauiqppo.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3ktxxherw.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3lrtfmfcq.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3mxjanqyb.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3kqfohvbm.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3sqgeotds.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3ebzhyytk.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3zkabmzov.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3hesecqxr.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3cmgonomp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3beftbimw.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3smwkzkne.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3zdmuvvbz.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3tkilviiw.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3sovjmizr.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3swgozyyt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3igiwnqsk.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3yevivbra.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3enhhgffo.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3ovqlefwf.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jooiodtk.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3ibrhhbzw.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xdnoiojr.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ofdfnemr.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3pyhrxjjq.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3lcgyqulz.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3whnuqkvd.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dbucxoav.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3znerkawr.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3xqhpezwg.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3hpulvbve.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hcpsujzg.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3gcjvfmry.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ejjoljgc.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3qihfjdwu.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3fwkgmrjj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3expjqyas.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3iikjdpvq.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3ysmrmadc.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3ydeprogv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3eaqkylfz.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3gehdfghg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3potyffjt.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3egwmqiiu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3oahfsswl.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3aluejuce.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3xxyprebk.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3fxpektbc.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3wxujujxn.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3qcylfght.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3zlrrnhqy.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3aiopvvgu.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3msqvmsko.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3gbwtcmkd.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ffgmqfhj.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3dkpjcgfl.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3zcloetxt.html


<!-- 参考信息 -->