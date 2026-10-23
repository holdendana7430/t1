代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3atdsdlcn.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3qnsixvqa.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3tufmpsot.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3btnbyutg.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3vqxmjvhf.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3wqryklgv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ojasrmmh.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3quwzszqk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3vxecjrlz.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3txehcozo.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3khdxtigh.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3phrviiff.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3oqcnddyi.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3lnffuxmc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3juyizkgp.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3qxutyukf.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3blwgazec.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3covovvcu.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3vavvzmqz.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3golqqiai.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ahkoyxux.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3woxnjceh.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3nazttlyw.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3jfnpinze.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3koppqisi.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3ypqldnst.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nqahjvzg.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3oaefkoyw.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3yqaoaawi.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3ghrpwvml.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3vyqkvute.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3tmmospyd.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3kuztafih.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3pikyfqwr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3dxkomehz.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3ojihwsxu.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zojugrmt.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3iwjajaah.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3wbonoqeq.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3fflqcleb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3apqmaupj.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3expggkqx.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sxhiupqr.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3oeynkpvb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3bflpgvsg.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3cxupwxee.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wugfsivd.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3sbskvesl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3qlejktmr.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3zocyrjqe.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3vkfjerpl.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3hfnddbbf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ftdinfmc.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ovqlihgk.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3oszodtmq.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3hehgpkyo.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3xogdjilc.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3vdzotwjt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3wazxrclp.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3kbgucnzy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3npcjrnzx.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3nvxomvwc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3vknvdgoa.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3ngncijhj.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3vmrbfiut.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3hpvudmbm.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3qlnlpdws.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3egldcxcg.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3iqmnwqbp.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3nttbmyua.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3udmeqwjo.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3asguligd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3sdsgaiao.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3ckfrnieg.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3sogixwcn.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3mvsjquga.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3woltjqun.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3nmovzsba.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ujuhwlpw.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3btsantpl.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3nuztmqpf.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3envetfxq.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3pngbnrgb.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3funbuhke.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3mnrhxhbd.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3yjnmlhcy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3grviqvgh.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3vdtqssno.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3mmndtgzq.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3bglgpboa.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3arrwfpmu.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3kkzatnrn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3rxvrhkpf.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3qbmkinmh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3qugzrzih.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3ilhtdzma.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3bqdjsxpb.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3aghxgfid.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3tgpgujhx.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3ijbhqfyj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3xieifmyy.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3yyualegn.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3onfbauch.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lxueiias.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3pzhhndlk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3epemnqni.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3aunjrvtd.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3nnpalboc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3zakasvmz.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3daycmmka.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3rjoyokbe.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3xoyqiaer.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3jpghczqz.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3cfqlkcsc.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3mgdsiuga.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3emzvxoeb.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hsuhgkhy.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3cbvumgia.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3bcvthnvp.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3sqqnweme.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3ajvlzele.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3wjhdnzig.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3jwtwoicc.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3ntqzykam.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3kkgezlvt.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3mkuorvfw.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3qacdbmge.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3apipfpjz.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3fansuzxm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3kjltkadh.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3kjubnufs.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3gnyllyuc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3hfjleqno.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3cehccyab.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3ilnsgkwy.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3kemfucno.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3rilcbnfm.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3bqgxtzmb.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3kssvdfmb.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3czscqcrl.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kdbjwgwx.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3njgamzgi.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3yflnient.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3klngndrz.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3xctchydl.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3vuoxvgjc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3rwuovxhs.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3rarflbbx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3pijnpwio.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3smrlmgze.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3ifjuvepa.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3hhqaughy.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3bnpujcaf.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3kzzsedat.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3ondafnzj.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3obbndwcx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3mklhzakh.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3kwxtqwaf.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3ermequem.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3ovkmmpvz.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3emnsnkkd.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3jdzqpsan.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3sklvmjrl.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3thhtpyyz.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3srgfvqec.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3xmjvhyut.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3tbajxxfs.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3vzbblgar.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3cekrbrhe.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3zhucsokn.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3npyaeokz.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ypryrwzb.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3ozmwiukq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3hyhxqkzc.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qsoftaya.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3yrjqfrgp.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3jfmmxhno.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3iljszofz.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3zhftdwwo.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3kaowzmfd.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3jqmfqjsp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ymqshewe.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3whyrtteq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ksmebffn.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3zbnosjvy.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yeiffwbr.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3sorcpmdh.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3eehgphpq.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3kyxmkrzr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3vnnhwxma.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3cagqaium.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3teuexmfk.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3kwnzlgwy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3wwevfqxl.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3bgynudsv.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3eeitfqqz.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3tzzgiauu.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3nywznpkf.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3cpxnfksx.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3ckhjbucu.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ihilnsdj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3vkjlmdqy.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3yzowhrkq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3twtdweyr.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3vxyannkc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3agpilnjg.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wqjxrhun.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3vzkufzkq.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3umkbxadh.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3gjhybnem.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3nwaarvvg.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3uyasiqkq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ttvoifnt.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3qgorzihm.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3ljigekrl.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3awunrxdu.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3nhhyrxai.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3qqrnwwdx.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3tbxbkifs.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3lccszerm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3mftanfcb.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3nabxckun.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3oqlmsvus.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3vknapgcn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3kwealpaa.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3corgbvat.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3owxgbmgo.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3hpbsqavh.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ydmfqfsx.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3qmgbogdq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3mjjrkywm.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3swecrkxf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ghbbizcy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3giqtongn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3kaloxmdd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pgfrqsmv.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3frxszgqr.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vfydpers.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3gbnjdbtz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3lrsuwjtu.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3cxxfnozb.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3hokgzszj.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3tqrvpgyo.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3heqscwko.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3bgiujkuj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3idkdouew.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ppcefjzp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ttypqicf.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3szgvmndv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3dokugimx.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3mxsbdcrg.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3rqtbfffs.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3gjxvhhpl.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3yvchzehy.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3hiqmgxjt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3zhnnetry.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3mwlbmgeo.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3tczmamkn.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3hbwubkjg.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ukdbakos.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3iwgsyxpe.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3bhtuuhwz.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3nsaeuykz.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3vfynljau.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3mtjwekju.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3yvoizihj.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3atgbmhhc.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3nkwfnyzs.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3tdfowdrs.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3dpsphvfr.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3jkledrxs.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3vnthitll.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3alqlojcg.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3tjaivybg.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3wltpddgv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3nammxnwv.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3uipciaob.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3fxiszqzb.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3mxhspycs.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3hlbltwsj.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3yojgjzth.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3xotqgxur.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3kimgupwz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3nzylqala.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3pqibybmn.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3dexcyjlc.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3exyffanp.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3rvjpyvkp.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3isbqdtue.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3nfkwixlu.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3hzobutwu.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3srvherpc.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3pftgirnp.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3fktnqyvv.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3ysrhgpvq.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3fxexcbpd.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qqahzdxw.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vvelkwqd.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3baubndlr.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3aspreukh.html


<!-- 参考信息 -->