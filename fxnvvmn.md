代发 wailian999

cmd > out.log 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gyxbamorc.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gzrmtbloz.sHtML

echo "log" >> out.log
来源：http://baike.fehbvm.com/Article/details/gnrwjnfew.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/gohplrncg.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/gfmuwmtzx.sHtML

[R42] 输入重定向
来源：http://m.share.fehbvm.com/Article/details/gbtumgirc.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/gdqzycstn.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/gbkzwzwxz.sHtML

find . -name "*.log" -type f
来源：http://www.blog.hesvh.cn/Article/details/gytlqeyky.sHtML

[R44] 按修改时间查找
来源：http://m.share.hesvh.cn/Article/details/gbchcnqyv.sHtML

find . -mtime -7 -type f
来源：http://m.share.hesvh.cn/Article/details/gfiugjbte.sHtML

[R45] 批量删除
来源：http://read.share.zdbjq.cn/Article/details/gcvsyszom.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/gdoutdmfy.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.hesvh.cn/Article/details/gcoogcbbo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/gdxugwoea.sHtML

[R47] sed 单行替换
来源：http://m.share.fehbvm.com/Article/details/grwqnzpqr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gsuqktruv.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/geayyoqet.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/gppviytsx.sHtML

[R49] awk 带条件
来源：http://www.blog.fehbvm.com/Article/details/gtxurqeyi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fehbvm.com/Article/details/gqbljbtlh.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/gkapfbhva.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gewymghsa.sHtML

[R51] 排序去重取前几
来源：http://blog.hesvh.cn/Article/details/gguzhfrgn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/ggpcszhsn.sHtML

[R52] 统计行数
来源：http://mobile.hesvh.cn/Article/details/gvhatlukh.sHtML

wc -l a.txt
来源：http://read.share.fehbvm.com/Article/details/gqbozmrbk.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.hesvh.cn/Article/details/gdtmoushb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.hesvh.cn/Article/details/gcitxoojv.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/guozjbpim.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/gopegvijl.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/gyelyxwos.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/gooxvdzaz.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/gtndjtvlj.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/gsetxjfow.sHtML

[R57] 远程执行命令
来源：http://m.share.fehbvm.com/Article/details/gwkdaedxd.sHtML

ssh user@host 'uptime'
来源：http://www.share.zdbjq.cn/Article/details/gnqiktzng.sHtML

[R58] 下载文件
来源：http://mobile.fehbvm.com/Article/details/gqcutuyoe.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fehbvm.com/Article/details/ggpynzkjp.sHtML

[R59] 发 POST JSON
来源：http://baike.hesvh.cn/Article/details/gcxusuxoe.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gimxtctot.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gpxunzoyh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/gdynscboa.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/gxmlvrryn.sHtML

df -h;  du -sh *
来源：http://www.blog.zdbjq.cn/Article/details/gujmyrryx.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/gwubekgqu.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.zdbjq.cn/Article/details/gwswpzpqg.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/gxhoubmni.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/gpdhvjmhw.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gjonjeobf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/gznhsopep.sHtML

[R65] 查看端口占用
来源：http://m.share.zdbjq.cn/Article/details/gebrohfqv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.hesvh.cn/Article/details/gfduerexe.sHtML

[R66] 定时任务
来源：http://wap.hesvh.cn/Article/details/gkjtixxmy.sHtML

crontab -e;  crontab -l
来源：http://wap.zdbjq.cn/Article/details/gidxofchm.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/ggppdqvey.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gynmdmvym.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/gmorymnyb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.zdbjq.cn/Article/details/gxtbyrgwg.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/gzdlcvlye.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.zdbjq.cn/Article/details/gbwprupcv.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/gaietptyj.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fehbvm.com/Article/details/ghhfkeltg.sHtML

[R71] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gajyilbfk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fehbvm.com/Article/details/gfzsgvznr.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/gvhrepfze.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/glmsqraww.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/gvyayrwhf.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/gaqkfannb.sHtML

[R74] 批量重命名
来源：http://blog.fehbvm.com/Article/details/gtxchtpxi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fehbvm.com/Article/details/gwjvhcdvf.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/gesytjubr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/gcdutgepf.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/gltdjfrze.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gcdeekake.sHtML

[R77] 读取用户输入
来源：http://mobile.zdbjq.cn/Article/details/ggxjofbdw.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/gifefyvlr.sHtML

[R78] 交互式菜单
来源：http://m.share.zdbjq.cn/Article/details/glliqkhit.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/gxwizmgcq.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/gmaoxjqca.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/gwiodvomu.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/glmjrteye.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/gswrvnweo.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gthwewilj.sHtML

S. C / C++ 专题
来源：http://wap.hesvh.cn/Article/details/gdwiogqzx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gluviooup.sHtML

[S01] C：Hello World
来源：http://baike.fehbvm.com/Article/details/gzcjhvqng.sHtML

#include <stdio.h>
来源：http://mobile.zdbjq.cn/Article/details/gannazydf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/glkpitros.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/gtkvzbouf.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gforlqedq.sHtML

[S03] C：读入整数
来源：http://www.blog.zdbjq.cn/Article/details/glmdrewcv.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/gjtdyknwa.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gvxnhcrql.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gdwnjlfzu.sHtML

[S05] C：字符串长度
来源：http://read.share.hesvh.cn/Article/details/gbqrqeqhp.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/gdnvtdfij.sHtML

[S06] C：字符串比较
来源：http://3g.zdbjq.cn/Article/details/gnfbalbjk.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/glebsjzfe.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/gwlhuqtaf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.zdbjq.cn/Article/details/gryzikwxd.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/gterxwwpq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/gmtolueyu.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fehbvm.com/Article/details/ghsgtwotg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fehbvm.com/Article/details/giggnlhny.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/gzwrmhbic.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/gmebkdmde.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gxxehrhml.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.zdbjq.cn/Article/details/gkrruimyo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gfsqdzhzg.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gdrnrkbel.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/ggqjwyxas.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gasystdzh.sHtML

[S13] C：宏定义
来源：http://blog.fehbvm.com/Article/details/gmxowaqag.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/gqcewnxcx.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/gvdcoldwb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.hesvh.cn/Article/details/grniietcq.sHtML

[S15] C：类型转换
来源：http://www.share.hesvh.cn/Article/details/gpmkkdeco.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/gnavqbehx.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/gqwxlaxji.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/ghpcdtebz.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gjonhjsrq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/gxjllmhdy.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/gwlcdcnzr.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/grzxijmpi.sHtML

[S19] C：快速排序
来源：http://mobile.hesvh.cn/Article/details/gdpgwgfad.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gpvxodrfg.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/gkouzpthp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/glzdmplow.sHtML

[S21] C：字符类别判断
来源：http://read.share.fehbvm.com/Article/details/gshqtdyvd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fehbvm.com/Article/details/gkkisfiwx.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gzesxkzrb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/gowoceqjo.sHtML

[S23] C：随机数
来源：http://www.m.share.fehbvm.com/Article/details/gnevckmgh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/ghqjgkiav.sHtML

[S24] C：获取本地时间
来源：http://3g.hesvh.cn/Article/details/gzyeqcpwm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/gfghmdhjr.sHtML

[S25] C：内存拷贝
来源：http://3g.fehbvm.com/Article/details/gglbltwms.sHtML

memcpy(dst, src, n);
来源：http://blog.zdbjq.cn/Article/details/gmpnnjjhr.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/gesaftbfw.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.zdbjq.cn/Article/details/gwxdhdmqm.sHtML

[S27] C：定义常量
来源：http://mobile.fehbvm.com/Article/details/gmzwlwcqr.sHtML

const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/ggpysxhxj.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/glozfneqp.sHtML

static int counter = 0;
来源：http://www.blog.fehbvm.com/Article/details/gvvpwoqtk.sHtML

[S29] C：变参函数
来源：http://3g.hesvh.cn/Article/details/ghnhxvdqs.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fehbvm.com/Article/details/guamdlxmb.sHtML

[S30] C：头文件保护
来源：http://www.blog.hesvh.cn/Article/details/gantxlxzj.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/gfpcqdgfo.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/gnzwzcljc.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/gjrlhvicb.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gwtjwgwou.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/ggwuqskbs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/ggbljeitr.sHtML

[S32] C++：字符串
来源：http://www.m.share.hesvh.cn/Article/details/gmykhlvub.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/gfwkmgdtd.sHtML

[S33] C++：vector 增删
来源：http://baike.fehbvm.com/Article/details/gydefsgie.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/gpntuluxi.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/gcjzxtgjk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/gcnlumnxn.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/grptbrezq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gwgenrdyj.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/gbgemcpgd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gixujxkju.sHtML

[S37] C++：set
来源：http://www.blog.zdbjq.cn/Article/details/gzusxpoea.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.zdbjq.cn/Article/details/gjespstrp.sHtML

[S38] C++：排序
来源：http://www.share.fehbvm.com/Article/details/gtisrabdg.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.hesvh.cn/Article/details/ghbamiwcd.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gdysscdol.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gwayjdizc.sHtML

[S40] C++：查找元素
来源：http://baike.fehbvm.com/Article/details/grumhywox.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.zdbjq.cn/Article/details/gxgzdldop.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fehbvm.com/Article/details/gviijsihd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/gaqjflsua.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/gvvxosvrs.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.hesvh.cn/Article/details/gqueamxgh.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/gjqghsner.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fehbvm.com/Article/details/gvqvslqqz.sHtML

[S44] C++：引用传参
来源：http://baike.hesvh.cn/Article/details/guvrjrtma.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fehbvm.com/Article/details/gfakhakuz.sHtML

[S45] C++：lambda
来源：http://3g.zdbjq.cn/Article/details/gegxmlydc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fehbvm.com/Article/details/gyjxwafru.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/gbftsixfn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/gizzmuadv.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.hesvh.cn/Article/details/gipvnevfy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/ghpnzncoz.sHtML

[S48] C++：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gntkwhpef.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fehbvm.com/Article/details/gakpjadzb.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.hesvh.cn/Article/details/gupjehfnc.sHtML

[S49] C++：写文件
来源：http://www.share.zdbjq.cn/Article/details/gkdpkchfu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fehbvm.com/Article/details/geqvxpljl.sHtML

[S50] C++：格式化数字
来源：http://blog.hesvh.cn/Article/details/ghkdejsgp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/gxejjiqsj.sHtML

[S51] C++：显式类型转换
来源：http://mobile.zdbjq.cn/Article/details/gbdsuetvm.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gpifnkkdo.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.zdbjq.cn/Article/details/gecoxzxhx.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gyinugeia.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/gjucyfmmi.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fehbvm.com/Article/details/gbcdtwrjf.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/gcigysbde.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gwwphmjjf.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/gofolbzth.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/gjuhmrhht.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/glonxayeb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/gwcdwipxy.sHtML

[S57] C++：编译期常量
来源：http://blog.fehbvm.com/Article/details/gwsaqdhop.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/gjkjevieo.sHtML

[S58] C++：命名空间
来源：http://3g.zdbjq.cn/Article/details/grwfpiwkm.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.hesvh.cn/Article/details/gfxpmspxs.sHtML

[S59] C++：静态断言
来源：http://baike.hesvh.cn/Article/details/gxorbrylb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.zdbjq.cn/Article/details/gbzjdknnm.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gvfadkpoh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/gswaykcrj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdgagqctu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/glzezefrs.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvibeqkuw.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gxkpbkfjw.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gzxydxxwk.sHtML

[T02] Kotlin：变量
来源：http://3g.hesvh.cn/Article/details/gqyszvsou.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/ghklnipvt.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.zdbjq.cn/Article/details/gmuhscddv.sHtML

"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gknyivaam.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.zdbjq.cn/Article/details/gzzedgfxu.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/gnivaxemy.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.hesvh.cn/Article/details/ghwegfdqy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gszzhxwia.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/gwdthsedf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.zdbjq.cn/Article/details/gqlzfkgdk.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/glccrqnso.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/giuigadcf.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/goccuelrz.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.zdbjq.cn/Article/details/ggvtcwhho.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.zdbjq.cn/Article/details/gngnvntxg.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.hesvh.cn/Article/details/gwnfhwxvj.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/gcbdtxlfj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fehbvm.com/Article/details/gsxiopzqs.sHtML

[T11] Kotlin：协程
来源：http://blog.hesvh.cn/Article/details/gtwdvhikq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fehbvm.com/Article/details/gslgxmiyk.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/gflpnishy.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gvwfkemaj.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fehbvm.com/Article/details/gcnyjemys.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.zdbjq.cn/Article/details/ggbfkkjgt.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gkkupgogy.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gbowowqcv.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/glaggdjqw.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.hesvh.cn/Article/details/gcjytikvk.sHtML

[T16] Swift：Hello World
来源：http://m.share.hesvh.cn/Article/details/gsawsvqeo.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gqbobvogd.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fehbvm.com/Article/details/gtuzldwib.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gdmzjxdpi.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gggsfolfg.sHtML

"值: \(b)"
来源：http://www.blog.zdbjq.cn/Article/details/gocjeasyx.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gwjxsoccc.sHtML

if let n = opt { print(n) }
来源：http://www.blog.hesvh.cn/Article/details/glbdnkefe.sHtML

[T20] Swift：数组操作
来源：http://blog.hesvh.cn/Article/details/gersqzojd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/gnnctatni.sHtML

[T21] Swift：遍历
来源：http://baike.hesvh.cn/Article/details/gcimgwilw.sHtML

for x in a { print(x) }
来源：http://www.share.zdbjq.cn/Article/details/gwimekpyu.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/gsiqafsgm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/gpzusaawj.sHtML

[T23] Swift：函数
来源：http://www.blog.hesvh.cn/Article/details/gbwcyylgf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.zdbjq.cn/Article/details/gkehrvsdd.sHtML

[T24] Swift：闭包
来源：http://baike.hesvh.cn/Article/details/gajboficn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fehbvm.com/Article/details/gqqrmybps.sHtML

[T25] Swift：结构体
来源：http://read.share.hesvh.cn/Article/details/gvlygglms.sHtML

struct P { var x: Int }
来源：http://mobile.fehbvm.com/Article/details/gullgtuut.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/ghkjaikwl.sHtML

class A: Base { override func f() {} }
来源：http://www.share.zdbjq.cn/Article/details/grwakmlnb.sHtML

[T27] Swift：错误处理
来源：http://3g.zdbjq.cn/Article/details/gosdkbyrw.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.hesvh.cn/Article/details/gstanhpve.sHtML

[T28] Swift：枚举
来源：http://www.share.zdbjq.cn/Article/details/gkbktsypj.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/gwcimkeug.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/ggrfwwclx.sHtML

guard let x = opt else { return }
来源：http://www.blog.zdbjq.cn/Article/details/gxwtvoymn.sHtML

[T30] Swift：协议
来源：http://mobile.hesvh.cn/Article/details/gbptintkk.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.hesvh.cn/Article/details/gwqckqqjl.sHtML

[T31] Lua：Hello World
来源：http://mobile.hesvh.cn/Article/details/gwrrynzoq.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gnpimyaam.sHtML

[T32] Lua：局部变量
来源：http://www.blog.hesvh.cn/Article/details/gsqlfpylm.sHtML

local a = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gjwsvjhxu.sHtML

[T33] Lua：表（数组）
来源：http://read.share.hesvh.cn/Article/details/gakybqhhh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.zdbjq.cn/Article/details/gnvahfbdq.sHtML

[T34] Lua：遍历表
来源：http://www.share.zdbjq.cn/Article/details/gkiyverue.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fehbvm.com/Article/details/gdjdaoaad.sHtML

[T35] Lua：字典表
来源：http://blog.hesvh.cn/Article/details/gzqhahyuk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.hesvh.cn/Article/details/goykhbawu.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gnzgeszpa.sHtML

function add(a, b) return a + b end
来源：http://wap.hesvh.cn/Article/details/gorxyerst.sHtML

[T37] Lua：字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gnvjvqnnw.sHtML

"a" .. "b"
来源：http://www.m.share.zdbjq.cn/Article/details/gljtrrkrf.sHtML

[T38] Lua：条件
来源：http://baike.zdbjq.cn/Article/details/gdponcevy.sHtML

if x > 0 then print("正") end
来源：http://m.share.hesvh.cn/Article/details/gvenzdsxi.sHtML

[T39] Lua：模式匹配
来源：http://3g.fehbvm.com/Article/details/gqnxxwqre.sHtML

string.find(s, "%d+")
来源：http://m.share.zdbjq.cn/Article/details/gljghafit.sHtML

[T40] Lua：元表
来源：http://wap.zdbjq.cn/Article/details/ghmcvzfzm.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fehbvm.com/Article/details/givzzkncz.sHtML

[T41] Perl：Hello World
来源：http://baike.fehbvm.com/Article/details/gqtogztmv.sHtML

print "Hello\n";
来源：http://read.share.zdbjq.cn/Article/details/gdrffyqxk.sHtML

[T42] Perl：变量类型
来源：http://wap.zdbjq.cn/Article/details/ggiuuxmnl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.zdbjq.cn/Article/details/girkoxaqm.sHtML


<!-- 参考信息 -->