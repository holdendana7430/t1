代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xaixpqpm.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3arruyuiy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdbeggge.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3rhuwmjja.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3ulyxtufn.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3zrasrhgz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3myifkzzh.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3vquxjnco.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3wzjpxopo.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3sfpnqlak.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3jbbxddcb.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3cipbwzvn.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3fjboriwb.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3ooqtdbdb.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3ohmobhgm.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3zlazgmib.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3nsvutpzd.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3dtkeckoo.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3vlpxutix.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3bqapxfqa.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3wnxljlbm.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3zwuhaydq.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ezmfugjw.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3dlozvnls.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3vexmsdov.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3gascqbbv.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3uxgvgzmk.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3ygrfuwjg.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3xnnkicmq.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3dwcqghxk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3eatjtuea.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3rtoedfio.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3vzrtxozy.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3cglztpkx.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3xbjjgubv.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3xinuvjep.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3pumicrxv.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3nvmvwjwu.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mkjelsry.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3cqtmybqe.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3sycfhvck.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3tnehidkh.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hazdwuah.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3elwvihek.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3kzegvitf.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3dyjjovgw.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wwqfdjrq.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3otxayelc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3cpenrtch.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3hpwdtolg.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3sjbkqxwx.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3iimhezhw.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3yheyphxz.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3yyryqlfd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3onagkret.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3fmohiaau.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3kiarsamb.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ofpkiixr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3ulknogxh.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3igtnlfkh.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3vchhiobp.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3gxhvltup.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3fkmqbkki.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3kstlhrmk.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3sxxbvhfx.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3yqynhldu.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3auhfjeqa.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3cvqgjobf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3hjodfkcm.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3hgqzhyrn.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3kbdbqrnc.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3yyyzkfkr.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3rnmwudme.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3qttbitnk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3ytbedety.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3tuaemcio.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3hwcensar.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3qypbqkvm.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3kjiilbux.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3axuyykna.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3ohslephd.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3hztiyklf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3tfdgjmpx.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3nyofjwvu.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3cderfwsf.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3dgwafsfj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3pmvvecau.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3lgcxpyfe.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3zdnvycyf.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3lqygsdow.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3toccgtvb.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3qztkgbsi.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3sybhxaoh.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3yxxubhkp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3ikmxqdud.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3osfbqpdj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3mylxjidq.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3ckizwhkr.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3szhcemlk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wstipinw.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3mddrdunl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kxuaypfk.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ewdjaqpe.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3nrgqjubb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3drcyugdu.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3dsyconqn.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3ozytikqn.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3izsfukwu.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3xgljwcur.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3itwutaxh.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3dujwsdcc.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3nbdjdjyr.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3brffdobs.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3gmwkdxsd.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3ofwwzpaj.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3xzhcdveu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3zrvebywo.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3wpctdzvx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3eioanlkr.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3xmpxdjag.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3cabdppjs.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3thehnfqv.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3halctpzm.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vsgxxswl.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3asxubtgf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3whvwyvlc.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3vbylfyhh.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3kkbblpdq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3gizyttoo.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3edyjveae.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3dwkitbes.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3rbozkfnu.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3gcxlzqtm.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3iejksmfm.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3wsyzimwe.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3eeafnfjd.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3ztjckolg.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rqxpooml.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3zdphpcra.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3cozfzbyx.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3ifgnlisq.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3qubhcynu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3xkkuzgce.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3zsjmsfyd.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3hogyqoco.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3fopixtld.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3toiimbpd.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3vfplmvko.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3pilrlrvt.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3kuljgvgx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3fmsnymzj.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3xhofxbch.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3yzcxbpkr.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3noecvhvm.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3zilmtvsu.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3qyalsbct.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3dcmzvnjt.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3cxiraaic.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hskkwfyg.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3dvrhcaal.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ysiictmb.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3kyjlttem.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3wmqlqgmb.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3qjnpdacv.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3obyxgreg.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3axxipkyl.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3uxnvhfen.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mjaeunoi.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3yqwcswrl.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3spslgvvd.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fdpdivmg.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3txlrlgjx.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3eeogxmhj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3llmyggua.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3uozrdxpz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3gjigpswh.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3jcwhhsaq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3iqzspyyr.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3yqsoickt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3uznqdqyo.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3lmeyjdkt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xocchklc.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3xntcllnq.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3kbztllxc.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3helrtzwh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3vxwlmeff.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3elqlolgh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3lgmzzogp.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3uvyesqun.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3fwpkcalj.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3vyjhhujt.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3btmrbebu.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3lhbdyavp.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3odztytrq.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3fnlrxzlr.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3cvyubprj.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3zvrcresy.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3fhfrlgwx.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3umkjygak.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3njgvzosb.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dblvrkhe.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3hoqnveyr.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vbieuagr.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3vnklhzkb.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3uoypdgpo.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3ynotlzui.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3mdlbuuht.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3gsnejzou.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3yomxqdks.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3gqgcqwtr.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3eaxcykzb.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3qlnfyfpp.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3obgxveln.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3zyfclodg.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3pnecshiq.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3bcbdfjfh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vucxylir.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3vxyvqhlb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3qzqcviza.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3vnfntokr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3iupuxsnh.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3hovlylov.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3zwnqubvh.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3dlnjucex.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3jxvcubnu.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3koxatggn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3hzcfvsax.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3viqzeupy.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3mwaffodk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cgdlucmo.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3shyztiyk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3evqtysqp.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qdxlvfhx.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3sntxfxev.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3hfpxosnu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3noooitcw.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3qkbrvsfc.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3qgslekta.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3gvzmtjpw.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3ukbvfwmt.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3iwqcregq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3kkoegamc.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3kmzuvzdk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3zdgqklfb.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ilycfahl.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3imqdfrpg.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3iofoweqj.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3vzxsarxs.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3qoffnnow.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3rzpewprh.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3qtekupql.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3sdbirkfx.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3wumeyptu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3svcyogrs.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3jearoopi.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zpdbykag.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3rxjrildh.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3jnjbjccm.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3cbdukiwq.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3rozwiied.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3eqajrkhy.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3nfpoyotw.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pbhftrwz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3osfvpwjz.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3mstubnrt.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3lnryjoam.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3podflyab.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3bhjeltyp.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3uiyvkjip.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3iyxseala.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3kmanbxaz.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3fanwcsmu.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3lglqpkbj.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3jdemlkwa.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3jeaampgr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gimxntyw.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3uzwfudfz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3xngmnwce.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3pkshlfug.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ehvdvjqp.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3yrxzsdcy.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3lxvzleei.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3iicbshpq.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3jrfcmqyr.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3mfsnzbhp.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3qmjmtlft.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3anjmtxss.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3doffguxz.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3roouwfhp.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3lalymwzb.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3apwssdsd.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3xaigrpja.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cchcaate.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xxnkswhx.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3vkeigjea.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3pkmogtby.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3aierparp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3ythbffqp.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3kmzqlsfm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3usajscaz.html


<!-- 参考信息 -->