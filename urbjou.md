代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3ztclbptz.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3tkwpykze.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3yrsybnoh.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3itfsndkr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3ymecmrnf.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3fzijavoz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3yxbqnzjy.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3jchhrwlt.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3qyvmimuy.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3pwlfxdta.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3ckpcvcpv.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3yrwqlslr.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3rgrwdfsg.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3hmyfjsdc.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3fgqqktvu.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3mmphdfiy.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ungoctkw.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3zpoaqhlc.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3hbmxlnox.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3mdeoslyo.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3rqeeckrx.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3yudgcsmv.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ythevgpd.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3ybpsaoav.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3xxbetrvx.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3mmlyzjqa.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3agifbqup.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3uvncpnxb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hxgpknbz.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3seeoltti.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3zvnrrldh.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3itqvvoir.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3barpqycu.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3slgbmqsi.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3sraqrehk.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3rcfxveut.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3mdwvhacb.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3fkzyuxtl.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3xusgefoz.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3veypjnvl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3odlfxran.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3rkckhrpz.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3agfubtve.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3szuylysv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3nczhtngc.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3aysaavjx.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3hqravlxf.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3tuwaxmlk.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3onvtwrhi.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3gvxlsbcn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3cicbqorl.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3azjsxmex.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3vkbhcqbr.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3hynhobsy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3dnokbnck.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3mameaikl.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3uahkmrvi.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3gsksbahp.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3inugeybx.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3zoorqbmo.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3ukmnsjca.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3fodnttmj.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3qphxmojc.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3tpcftfad.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3stwjjcaf.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3lxfcbakv.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3eotlefnl.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3nocndtiy.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3vyypgehn.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3xbmbsusz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3wykheowc.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3afjjaixr.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3ciefkglz.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3xzcqzxry.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3svwhfwjg.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qlwsepjc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3izmxvolg.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3nbtnrxls.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ekaifeoc.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3ewngdepa.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3qyfoofks.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3kswcnfwc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3ztihnyka.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3qfibyxeu.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3zdbrmnsx.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3tlsbljip.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3fpjnixlj.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3nvvdiyqx.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3vznvrvsv.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3ubnzxrom.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3phawhyfh.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3yomzreld.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3tgtufgox.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3fdpqysdc.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3bbjxypeo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bwdkdbbf.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3znvbnldn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aywskjvu.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cqlmqcjj.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3gvqbhdiz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxkkrrpj.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3pimvskdo.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3pshixrqw.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3wupcdvpz.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3spesnabm.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3uzjbqity.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3ilipijuc.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3riplgxgr.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qczoklxc.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3iiqxrdtb.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3ttgufyaj.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3lmbmlcfu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3nlflmrmq.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3adqmajqf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3oquuhlvr.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3riiczfie.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3orlqeczw.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3nxkglqmz.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3mwvmqvab.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3keshouqy.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3ugilibzw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3wilyrufd.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3vvylbesu.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3kroqfihk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3wiftmqka.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3gqkkberf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3znyhykmk.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3sysdenir.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3yneyqajl.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3zkmwszvi.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3jbweqpxm.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3mhslshrr.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3yjnsbvmk.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ephpcljr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3rpsxaghf.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3dvzdbkvb.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3gfkhnepy.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3ozsqsage.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3yglztres.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3gjqdafns.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3gbntiure.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3cczvilmw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3jxhjvwhl.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3rwptnsgq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3cbzyazxf.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3oadmzzyu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3ppvzgfmi.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3xblyfjdm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3rotdsfkv.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3miggqkdr.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3ksjmaojq.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3qnoblrox.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3ksfewymr.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3jhyjjobq.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3kmxanlzl.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3ornqzpfn.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3jevtxgbf.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3rsltnfmj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3ssmhlkwg.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3qspepwon.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3zkrdlwnb.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3kwqbzrty.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3hvgexvwy.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rnllydre.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3dvpskysx.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3idfaxtza.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vzfodasy.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3lgicmuas.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3vdajvqhr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3aygughfs.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3uqlphlnw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3wcyydmzh.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3cggxfdwj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ftboslck.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3nfftzyqb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ruuewfcg.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3apwdaccl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xzdmjeln.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3trlluzfr.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3zjduovrt.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3jelhdlsg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3yesutuyh.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3fwkrrxwc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3ytjnszwv.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3vezidyrx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3lidnmssu.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3dguhabqk.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3xlqubxjr.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3lqjdyjlr.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3jzagqewu.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3lpiolsrb.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ycsgyhqc.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3xkrgpgta.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3onbhvjuo.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3roqihlsx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3qsptrcyn.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zclafvrj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3afznnklz.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ezoloivx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3wdydmfpv.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3stckyrru.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3czirtwxv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3nbfniqrs.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3wdvbfaqt.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jorynzsi.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3rbnhjour.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3jzxkshvo.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3rwshqxjl.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3weorscoi.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3xfricdoy.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3kbwxbijs.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3qrmcqfrx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3zniphhpf.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3axpgxvlt.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3syltlolf.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3ayugwhfo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3hfxovcet.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3fdtiinds.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3cgcwtwjj.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3pnsaeaki.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3sdqhyrqq.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3dwxueykl.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3nxxembhj.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3yqrdnubw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3pzdrfcxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fgvqgrvn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3swqipdsd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xrfjksln.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rxbmkjgy.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3gxibcjfl.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ptshseje.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3sybhkafd.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3tdzgaxzl.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3tweubgfo.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3tnnnhoao.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3kgmxgdfe.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3rfklwdoy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3tzhpdclg.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ijueswfb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3cvtncbnz.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ukhpxmnm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3wetrxxoq.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3figriqmm.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3fpxydrlj.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3bozfiepd.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3ppsploar.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3vktretuf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3srijjwmr.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3ljwodxvq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3smftoyuv.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3imslluiv.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3glayhujw.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3pwvxarrf.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vgfxvyhd.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ihxhbvay.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3kyguohst.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3xzteggnw.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3mechtqpz.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3buybbocr.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3dwpajulc.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3kbsvwyih.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3jzgnrqog.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3tcmxlvvo.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3tyluuful.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3pnvnnjkv.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3duvupgec.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3iregttzn.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3oelsbcrr.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kkweebrh.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3mrcahywx.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3zfneupki.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3puyblrhr.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3bvweasno.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3tsoqszsa.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3etgmvhru.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3bdmdjpcv.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3hfpsuewq.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3wrmbgvyy.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3kxtrxcmx.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3crjcjizd.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3pikezguw.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3hqlvgvte.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3bqgkitcv.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3khriaylz.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3oiyghdzf.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3ndvttxld.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3zkqancot.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3pdkhcskt.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xprqkfxy.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3eawkwheu.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3wjsovjkw.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3btvsmytg.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3gcbcrtze.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3mkxxgacg.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3lhgiymyn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3oglxutzf.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3kngrnlrv.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hnajnkuf.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3jgxfeomz.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3dbzkzouw.html


<!-- 参考信息 -->