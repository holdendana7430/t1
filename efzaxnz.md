代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.hesvh.cn/Article/details/gcchdclzv.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gddaazpqv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gciomfzqp.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/gzyepkzyr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.zdbjq.cn/Article/details/gfejylnbx.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.hesvh.cn/Article/details/gwldeciap.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.zdbjq.cn/Article/details/gqcsihyxc.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/gsuottlyw.sHtML

files=$(ls -1)
来源：http://www.blog.fehbvm.com/Article/details/gsttpnmct.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/guwrknofe.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/gxnuuldiy.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.hesvh.cn/Article/details/gfamrgios.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/gxxswlvkl.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/gvyxqjqke.sHtML

echo "log" >> out.log
来源：http://baike.fehbvm.com/Article/details/gzcutxjnk.sHtML

[R41] 丢弃输出
来源：http://www.m.share.zdbjq.cn/Article/details/giohzmkty.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gazzgamup.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/ggjwiscaj.sHtML

wc -l < a.txt
来源：http://read.share.fehbvm.com/Article/details/gvvasjffh.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/gqbineqzv.sHtML

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/gshhaynua.sHtML

[R44] 按修改时间查找
来源：http://3g.hesvh.cn/Article/details/gkgxtotdh.sHtML

find . -mtime -7 -type f
来源：http://3g.zdbjq.cn/Article/details/gjqdjfork.sHtML

[R45] 批量删除
来源：http://www.share.hesvh.cn/Article/details/gglbckbno.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fehbvm.com/Article/details/glygcssfa.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/grjqqtgvu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.hesvh.cn/Article/details/gqbreljfe.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/gsjuclqoq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fehbvm.com/Article/details/gmqqbewtz.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gqycfnkad.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gbkofhwir.sHtML

[R49] awk 带条件
来源：http://m.share.fehbvm.com/Article/details/gyytfeczx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/gkguxhkgk.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/gwnyhygmz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/ganugspkv.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/gcnehqruh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fehbvm.com/Article/details/gphdwsvat.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/gvgkoermt.sHtML

wc -l a.txt
来源：http://baike.fehbvm.com/Article/details/gavmqvski.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/gnfpbqngn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/gkkbqjwek.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/gpemleius.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/gonvulklz.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/gtpddntif.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gstyexccv.sHtML

[R56] 远程拷贝
来源：http://baike.hesvh.cn/Article/details/gadjoombv.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/gdihtfbsn.sHtML

[R57] 远程执行命令
来源：http://read.share.zdbjq.cn/Article/details/gkkrpfdng.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/gkmxtmyia.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gqnbwzzdr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/gwrdvvrsr.sHtML

[R59] 发 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gplvmhmkv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fehbvm.com/Article/details/ggsucetrn.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/guwzvavkr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.zdbjq.cn/Article/details/gnprncihi.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/gnxexroop.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/gfptolgqk.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/gucqosqho.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/gjllreyds.sHtML

[R63] 内存与进程
来源：http://mobile.zdbjq.cn/Article/details/gdaihqmuc.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/gfekczlhi.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/gbbmzbhos.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/gmndldwnh.sHtML

[R65] 查看端口占用
来源：http://www.m.share.zdbjq.cn/Article/details/gpchdfewp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.hesvh.cn/Article/details/gczypxswm.sHtML

[R66] 定时任务
来源：http://blog.fehbvm.com/Article/details/ghsunzvxc.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/gzxntvcog.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.zdbjq.cn/Article/details/gdqbyjigo.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/gqdkmwuqp.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/grcttcgra.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gphftjkrk.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fehbvm.com/Article/details/gzzljcwkq.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/gngbonevi.sHtML

[R70] 时间戳与互转
来源：http://www.share.hesvh.cn/Article/details/gddhwbrjc.sHtML

date +%s;  date -d @1700000000
来源：http://wap.hesvh.cn/Article/details/gqmemxijd.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gopuriwss.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fehbvm.com/Article/details/gsqfycurk.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/gdlspiphy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/ggpiccmoh.sHtML

[R73] 分割大日志
来源：http://www.m.share.zdbjq.cn/Article/details/ghzkzrdrt.sHtML

split -l 1000 big.log part_
来源：http://wap.fehbvm.com/Article/details/gxhuepxkj.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/gefosvbzk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.zdbjq.cn/Article/details/gxshlmtoq.sHtML

[R75] 导出环境变量
来源：http://mobile.fehbvm.com/Article/details/gdcbcyzke.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.zdbjq.cn/Article/details/gxijbaoij.sHtML

[R76] 使用临时文件
来源：http://baike.fehbvm.com/Article/details/glimqwgly.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gcbviibmp.sHtML

[R77] 读取用户输入
来源：http://www.blog.fehbvm.com/Article/details/ggpqwxxmt.sHtML

read -rp "请输入: " ans
来源：http://wap.fehbvm.com/Article/details/ggcbtfamf.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fehbvm.com/Article/details/goimfgwdd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/gxzkypvvq.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/gsxhkqxcb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/gkbbgyhii.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.hesvh.cn/Article/details/gavuztzay.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/gdoxchxid.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqjjwlmly.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/gjinnvzeh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gttomdngk.sHtML

[S01] C：Hello World
来源：http://baike.zdbjq.cn/Article/details/gfidfkfcc.sHtML

#include <stdio.h>
来源：http://baike.zdbjq.cn/Article/details/gqlyboyin.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fehbvm.com/Article/details/gosqhlphx.sHtML

[S02] C：变量与格式化输出
来源：http://wap.hesvh.cn/Article/details/ggnnecbwe.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.zdbjq.cn/Article/details/gmfjjfrsa.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/gkgnhcrba.sHtML

int x; scanf("%d", &x);
来源：http://www.share.zdbjq.cn/Article/details/gfkgrgavq.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gxejfcneb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/guxxlzilz.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/goedmbsru.sHtML

strlen(s)
来源：http://www.blog.fehbvm.com/Article/details/gsljjsmmo.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/gnimutkib.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/gkyrcztqt.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/gpuqflwba.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/glpntedqy.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/gkwnvxacy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fehbvm.com/Article/details/gsplvdjoo.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/grtqsvrnz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/grltpvrdq.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/gochalhst.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.hesvh.cn/Article/details/gpfewhkeg.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gmathluwy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.hesvh.cn/Article/details/gjrhjefhe.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/golixqsxt.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gumdnhipj.sHtML

[S12] C：写文件
来源：http://3g.fehbvm.com/Article/details/gycuscwvn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gtysujyab.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/gwcodgqky.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/gatssvknt.sHtML

[S14] C：枚举
来源：http://www.m.share.fehbvm.com/Article/details/glheaisni.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/gosscdmyz.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/gpimqagfb.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/ghbxolpch.sHtML

[S16] C：位操作置位
来源：http://baike.hesvh.cn/Article/details/guswlraqt.sHtML

x |= (1 << 3);
来源：http://wap.fehbvm.com/Article/details/gtazhtnod.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gmfwdkxnm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/gggunagjs.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gszncjvzm.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/gfiogxtvl.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/grnbquxka.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gcsvdhnel.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/gcujsgwxk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gpfpqqeiw.sHtML

[S21] C：字符类别判断
来源：http://3g.zdbjq.cn/Article/details/gyvksriry.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/gcnawucij.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gcifygimr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fehbvm.com/Article/details/gfvnshbze.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/gqixxdvar.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fehbvm.com/Article/details/gbynlniqp.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/grtaiezcb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fehbvm.com/Article/details/gnmgsdeqj.sHtML

[S25] C：内存拷贝
来源：http://baike.hesvh.cn/Article/details/gkuqkktre.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gkzannbbo.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/gnyuthyiy.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/gxhaszmdw.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/getileayb.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gbbneundn.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/ggduliuuf.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/giubymsjo.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/gfujwnmnc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fehbvm.com/Article/details/gjobodoks.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/gohozfnkv.sHtML

#ifndef X_H
来源：http://baike.hesvh.cn/Article/details/grfprawat.sHtML

#define X_H
来源：http://www.share.hesvh.cn/Article/details/gcfepuinz.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/ggzcndntm.sHtML

[S31] C++：Hello World
来源：http://blog.fehbvm.com/Article/details/gmrwsdusj.sHtML

#include <iostream>
来源：http://www.m.share.fehbvm.com/Article/details/gcgrlczhm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/gvsddctua.sHtML

[S32] C++：字符串
来源：http://baike.fehbvm.com/Article/details/gtsbpdhgr.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gtiodsywo.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/gqawaaxyu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fehbvm.com/Article/details/grmqgpmct.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/gkzcwqjcq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.zdbjq.cn/Article/details/gdbxlrqra.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gtbxsyqzr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gpapzgwxu.sHtML

[S36] C++：unordered_map
来源：http://wap.hesvh.cn/Article/details/gnrmgdbnq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/glfvcqant.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/gghzlffor.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fehbvm.com/Article/details/gbrmrttle.sHtML

[S38] C++：排序
来源：http://blog.hesvh.cn/Article/details/gqrsdopkk.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gwnewffla.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.hesvh.cn/Article/details/gkosdnpxy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.hesvh.cn/Article/details/gdkdrxouy.sHtML

[S40] C++：查找元素
来源：http://m.share.zdbjq.cn/Article/details/ghvzubjsb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fehbvm.com/Article/details/godfedzvb.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/ggpbdpifq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/gynzzdxir.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.hesvh.cn/Article/details/gghogeujs.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.zdbjq.cn/Article/details/gwaycszlk.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/gmprgvwrd.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.hesvh.cn/Article/details/gtnfkwthp.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/ggrjtkrdw.sHtML

void inc(int &x) { ++x; }
来源：http://wap.hesvh.cn/Article/details/gloosexte.sHtML

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/gxkyxtduz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.hesvh.cn/Article/details/gikhcorrd.sHtML

[S46] C++：函数模板
来源：http://www.share.fehbvm.com/Article/details/gxyipramp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.hesvh.cn/Article/details/gdrbcfkzb.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.zdbjq.cn/Article/details/gtrkggifl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/ggfplqqyd.sHtML

[S48] C++：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gygqtjqpi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.zdbjq.cn/Article/details/ghxysxtzr.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/gyjrhblhx.sHtML

[S49] C++：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gintupttd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.zdbjq.cn/Article/details/gglmprkys.sHtML

[S50] C++：格式化数字
来源：http://www.share.fehbvm.com/Article/details/gffkmaqbk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fehbvm.com/Article/details/gpydonrdu.sHtML

[S51] C++：显式类型转换
来源：http://blog.fehbvm.com/Article/details/gepjztiof.sHtML

static_cast<double>(a) / b
来源：http://read.share.hesvh.cn/Article/details/gygmpotce.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/griuuqbkg.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gusidqpbv.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/ghfpglfca.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/gpkyxqlqz.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/glcctdmiw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.zdbjq.cn/Article/details/guesojxya.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/ggfddsuyw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.hesvh.cn/Article/details/geptgtkfl.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/gnvhgdnhi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fehbvm.com/Article/details/gnhdviurs.sHtML

[S57] C++：编译期常量
来源：http://3g.fehbvm.com/Article/details/gillkiddp.sHtML

constexpr int N = 10;
来源：http://mobile.fehbvm.com/Article/details/gomzssgfr.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/geaymovvr.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/geritmlrg.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/gbpzqlwvr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/godwxyanx.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fehbvm.com/Article/details/glaixbhbx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gzpnsxoof.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glguhdhgu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gbpwrjbcs.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzxskikfm.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fehbvm.com/Article/details/gvqcbdoix.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gclkgiibx.sHtML

[T02] Kotlin：变量
来源：http://wap.zdbjq.cn/Article/details/gchueabig.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.hesvh.cn/Article/details/guhyumjls.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.hesvh.cn/Article/details/gvoszpvaj.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gwyykuyih.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/gkguvhddq.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fehbvm.com/Article/details/gfxngpfgn.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.hesvh.cn/Article/details/goyalmikh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/gioxviqtr.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fehbvm.com/Article/details/gubrvkpiy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.hesvh.cn/Article/details/goskpvwrw.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/ghwvqbfcb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.zdbjq.cn/Article/details/giavwpiqb.sHtML

[T08] Kotlin：数据类
来源：http://baike.zdbjq.cn/Article/details/gnyixumgy.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/gogxxxlkk.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.zdbjq.cn/Article/details/gaaqdfisz.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fehbvm.com/Article/details/guvchydgt.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gzlqafvpa.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.zdbjq.cn/Article/details/gzfnbwmzh.sHtML

[T11] Kotlin：协程
来源：http://3g.zdbjq.cn/Article/details/gszltoybf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.hesvh.cn/Article/details/gbijupaey.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/gbdveeubh.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fehbvm.com/Article/details/gelmpppgh.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/gmhtdfkje.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.hesvh.cn/Article/details/gmguplwpd.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/gpkcokiqo.sHtML

for (i in 1..10) println(i)
来源：http://baike.fehbvm.com/Article/details/glppavjue.sHtML

[T15] Kotlin：接口
来源：http://m.share.hesvh.cn/Article/details/gimzcgoek.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fehbvm.com/Article/details/gplwgqwwo.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gglygoypv.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gfxsehbiy.sHtML

[T17] Swift：变量与常量
来源：http://mobile.zdbjq.cn/Article/details/gxtzicehu.sHtML

var a = 1;  let b = 2
来源：http://blog.fehbvm.com/Article/details/gstovuvjk.sHtML

[T18] Swift：字符串插值
来源：http://blog.hesvh.cn/Article/details/gemehuppf.sHtML

"值: \(b)"
来源：http://3g.fehbvm.com/Article/details/gsedejmlf.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fehbvm.com/Article/details/gazkdgxvp.sHtML

if let n = opt { print(n) }
来源：http://baike.hesvh.cn/Article/details/gtvkojnrm.sHtML

[T20] Swift：数组操作
来源：http://blog.hesvh.cn/Article/details/gvwosjhab.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fehbvm.com/Article/details/gohfxkgny.sHtML

[T21] Swift：遍历
来源：http://baike.fehbvm.com/Article/details/gtceqysih.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/gfzawemsj.sHtML

[T22] Swift：字典
来源：http://m.share.fehbvm.com/Article/details/gqvwlwvkf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fehbvm.com/Article/details/ggzhgokmx.sHtML

[T23] Swift：函数
来源：http://www.blog.fehbvm.com/Article/details/gegwofjlh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fehbvm.com/Article/details/girxihyyi.sHtML

[T24] Swift：闭包
来源：http://www.m.share.hesvh.cn/Article/details/gwoytfydh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gohxrsixa.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/grpqcdnlf.sHtML

struct P { var x: Int }
来源：http://blog.hesvh.cn/Article/details/gzqeqwrkd.sHtML

[T26] Swift：类与重写
来源：http://mobile.zdbjq.cn/Article/details/ggekrmlnf.sHtML

class A: Base { override func f() {} }
来源：http://3g.fehbvm.com/Article/details/gffgoxvlc.sHtML

[T27] Swift：错误处理
来源：http://read.share.fehbvm.com/Article/details/gxdpgltdi.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fehbvm.com/Article/details/ghyqaeeae.sHtML

[T28] Swift：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gemcbxacu.sHtML

enum Color { case red, green }
来源：http://www.m.share.zdbjq.cn/Article/details/goprljjsx.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fehbvm.com/Article/details/gqleocfak.sHtML

guard let x = opt else { return }
来源：http://wap.fehbvm.com/Article/details/givdfimvz.sHtML

[T30] Swift：协议
来源：http://read.share.zdbjq.cn/Article/details/gpvwspxmv.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fehbvm.com/Article/details/gtpfapyod.sHtML

[T31] Lua：Hello World
来源：http://blog.zdbjq.cn/Article/details/gggrdcmbo.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gogjoznvb.sHtML

[T32] Lua：局部变量
来源：http://wap.hesvh.cn/Article/details/gyyuhvzcs.sHtML

local a = 1
来源：http://mobile.hesvh.cn/Article/details/gsnlybvil.sHtML

[T33] Lua：表（数组）
来源：http://wap.zdbjq.cn/Article/details/gctcnmoxq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/ghzqaaxdh.sHtML

[T34] Lua：遍历表
来源：http://www.share.hesvh.cn/Article/details/gnmhntgnt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fehbvm.com/Article/details/goezfftvo.sHtML

[T35] Lua：字典表
来源：http://3g.fehbvm.com/Article/details/guhwxvtpn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.hesvh.cn/Article/details/gxabdyibe.sHtML

[T36] Lua：函数
来源：http://read.share.hesvh.cn/Article/details/gutweewqb.sHtML

function add(a, b) return a + b end
来源：http://mobile.fehbvm.com/Article/details/gqvwfgcgq.sHtML


<!-- 参考信息 -->