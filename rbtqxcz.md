代发 wailian999

find . -name "*.log" -type f
来源：http://www.blog.fehbvm.com/Article/details/gtkwhkaua.sHtML

[R44] 按修改时间查找
来源：http://m.share.hesvh.cn/Article/details/gdtinbwfj.sHtML

find . -mtime -7 -type f
来源：http://www.blog.zdbjq.cn/Article/details/gzrrixkkh.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/gzdlgsrcq.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/gsgtrkpgb.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/gjjgguepk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/gxznuuarn.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/ggykvmxig.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/gaosofutb.sHtML

[R48] awk 取指定列
来源：http://www.blog.zdbjq.cn/Article/details/gpuvpnogy.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fehbvm.com/Article/details/gaknlmtou.sHtML

[R49] awk 带条件
来源：http://www.blog.fehbvm.com/Article/details/ghwnkpjzi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/gfqjyppwu.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/gfknwrzxd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.hesvh.cn/Article/details/gwtfxzepe.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/gblsbkrht.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/gidhlcxtk.sHtML

[R52] 统计行数
来源：http://mobile.hesvh.cn/Article/details/gnkzfenuz.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/gymuzhetd.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/ggqretrbn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/gdybrtqjj.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fehbvm.com/Article/details/ggngllbzy.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/gdkpaidip.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/gqcidiern.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.hesvh.cn/Article/details/gpnbsdpzr.sHtML

[R56] 远程拷贝
来源：http://3g.zdbjq.cn/Article/details/gihyajtif.sHtML

scp file user@host:/path/
来源：http://m.share.zdbjq.cn/Article/details/gkdfgnohl.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/gtvtfbxes.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/gdalhpjlz.sHtML

[R58] 下载文件
来源：http://baike.zdbjq.cn/Article/details/gxagyczeu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fehbvm.com/Article/details/gvkymgsrk.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gdnpasjzj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/gmceczirz.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gjxcmjogw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/gvnxeaoek.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/gpdrgoeku.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/gjwdwkzyk.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/glzgjuiuz.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/gayydpbhy.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/gqamzrhoo.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/ggjxqzlnw.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/gacdnysbz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fehbvm.com/Article/details/gkhzuqraz.sHtML

[R65] 查看端口占用
来源：http://www.share.fehbvm.com/Article/details/gtvkpqhzc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/gebhmbccb.sHtML

[R66] 定时任务
来源：http://3g.zdbjq.cn/Article/details/gwlhntyki.sHtML

crontab -e;  crontab -l
来源：http://blog.hesvh.cn/Article/details/gucefkhmm.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/gngxbnuwj.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/ggdfaimmc.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/gspwsidky.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.zdbjq.cn/Article/details/ggctzkdua.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/geiegrpno.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fehbvm.com/Article/details/gatuzgoar.sHtML

[R70] 时间戳与互转
来源：http://www.blog.zdbjq.cn/Article/details/gblhxxdwm.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/glcioasyo.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/ghhxjrevg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/gklfjuvkw.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gwdvytuxt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gtryryrow.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/ggmyybvre.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gvxjexpao.sHtML

[R74] 批量重命名
来源：http://www.share.hesvh.cn/Article/details/gipeyacta.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.zdbjq.cn/Article/details/gfcgbbcew.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gmzjvjfmz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fehbvm.com/Article/details/gcbqjovdf.sHtML

[R76] 使用临时文件
来源：http://wap.hesvh.cn/Article/details/gkhslumzz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/grqeucbbr.sHtML

[R77] 读取用户输入
来源：http://mobile.fehbvm.com/Article/details/gkmbfmcty.sHtML

read -rp "请输入: " ans
来源：http://3g.zdbjq.cn/Article/details/gjqmdowpc.sHtML

[R78] 交互式菜单
来源：http://wap.fehbvm.com/Article/details/gdocsvhwm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/grsbmxxie.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/gyanvoeif.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fehbvm.com/Article/details/goqikhfxg.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/gwngdijxp.sHtML

time ./run.sh
来源：http://www.share.hesvh.cn/Article/details/gtqwxtoba.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqjerjpxs.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/gmxsqslgc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwmtzkudh.sHtML

[S01] C：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gcajsrgav.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/gmaphnysb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.hesvh.cn/Article/details/gzvmxneid.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/gipraqfcx.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gflmjuvxv.sHtML

[S03] C：读入整数
来源：http://baike.zdbjq.cn/Article/details/gimcelvcb.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/gyrlrydtf.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/ghsoklxpc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.hesvh.cn/Article/details/gcuvhphky.sHtML

[S05] C：字符串长度
来源：http://blog.hesvh.cn/Article/details/gswohvdet.sHtML

strlen(s)
来源：http://www.blog.hesvh.cn/Article/details/gzusfysgk.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/grdttpktf.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/gtahybppf.sHtML

[S07] C：数组遍历求和
来源：http://wap.fehbvm.com/Article/details/glkgilfbv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/gqasoshlq.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/gqatjiuae.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/guypenytu.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/gfwiyasnp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/gzjgrcayr.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gnolhooob.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/gtaxbwjlr.sHtML

[S11] C：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gavxkqhbg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.hesvh.cn/Article/details/gqllsomlt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.zdbjq.cn/Article/details/gluizjzzu.sHtML

fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gwzarwvko.sHtML

[S12] C：写文件
来源：http://blog.fehbvm.com/Article/details/glfzthrqh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/gsakekcuo.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/geovqqcdo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/gzswivazo.sHtML

[S14] C：枚举
来源：http://3g.fehbvm.com/Article/details/gchoeuttf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.zdbjq.cn/Article/details/gfjhkdtfr.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/gnoufdvyj.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/gmpxqvbgb.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/gelxuexiu.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/gjdbucxoq.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gvybqrqbi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/giikmxhku.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/glcpauzeb.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/gxhglgark.sHtML

[S19] C：快速排序
来源：http://mobile.zdbjq.cn/Article/details/gwjxkhlff.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gkmskibvc.sHtML

[S20] C：二分查找
来源：http://blog.zdbjq.cn/Article/details/gforzhhrj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gfzieggys.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/gxadbdcuy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/gqldegxpi.sHtML

[S22] C：字符串转数字
来源：http://mobile.fehbvm.com/Article/details/gwkjidgep.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/gvqkouwiq.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/gmcopqouu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/ggfdfjcfg.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fehbvm.com/Article/details/gkmxxwmrg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.hesvh.cn/Article/details/gfwofzoxp.sHtML

[S25] C：内存拷贝
来源：http://m.share.hesvh.cn/Article/details/gxldpsdxb.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/glrrcprur.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/grlydfvmt.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/gcvafavuy.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/gieavdfnd.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gdexujyus.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/gcismuqfh.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/gozjydukv.sHtML

[S29] C：变参函数
来源：http://blog.zdbjq.cn/Article/details/gufhmrllm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gkfecmwil.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gzfgprgrk.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/gnzpnevpu.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/gmcvkiwyu.sHtML

#endif
来源：http://blog.zdbjq.cn/Article/details/gcbhsdgnb.sHtML

[S31] C++：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gaocjahcd.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/ghlqsvohl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/gietcjqnm.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/gvsbfgbvl.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/glfpurwuc.sHtML

[S33] C++：vector 增删
来源：http://mobile.zdbjq.cn/Article/details/gscnevcfp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gsqnrdtly.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fehbvm.com/Article/details/gnocorvnq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/glnpzamls.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/gtbtsxvgq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gdvwoehrl.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/gcogjlkbr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/ghwjrzvlw.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/geayhozjw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/gppikrczv.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/gpdlgptzl.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/gsdbybuuk.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/grwrgqbaf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/gmvxmwduz.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/gebpqtwyi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.zdbjq.cn/Article/details/gytouyakf.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/gwpdiwgnv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.hesvh.cn/Article/details/gzxtvqugk.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/gcvatdibx.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.zdbjq.cn/Article/details/goytxycjf.sHtML

[S43] C++：智能指针
来源：http://m.share.hesvh.cn/Article/details/glhxjlulh.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/glyaontwg.sHtML

[S44] C++：引用传参
来源：http://m.share.zdbjq.cn/Article/details/ggzbeduye.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/gwovkfjzf.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/gnmqzmjxc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/gotnaqlgp.sHtML

[S46] C++：函数模板
来源：http://baike.hesvh.cn/Article/details/gcegwwszv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/gpnnvpfeb.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.hesvh.cn/Article/details/gzlkyuado.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/ghfaxadmd.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gxxgnmoza.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fehbvm.com/Article/details/gozerjnve.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/gaidetmll.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/gpyvoinpv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.hesvh.cn/Article/details/greythcmb.sHtML

[S50] C++：格式化数字
来源：http://read.share.zdbjq.cn/Article/details/glvhrjqig.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/gkcnlzzej.sHtML

[S51] C++：显式类型转换
来源：http://mobile.hesvh.cn/Article/details/gwvbgkwak.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/gznvswhwv.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/gtzifddal.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/gmtaqsvou.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/gvtquudnm.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/gvleydozd.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/gadktrfyw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gzzutbcat.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fehbvm.com/Article/details/gegcelelp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/gthufdqbe.sHtML

[S56] C++：optional
来源：http://www.share.zdbjq.cn/Article/details/gdotsctgg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/gfohewpop.sHtML

[S57] C++：编译期常量
来源：http://read.share.fehbvm.com/Article/details/gbzhzvxfc.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/gdaeooftm.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/gqnfznrfs.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.zdbjq.cn/Article/details/gxkvgkzui.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/gmcunftlu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gqswgywxr.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/gulrdinaa.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fehbvm.com/Article/details/gkqptsowe.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gttbultav.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gyviqdfap.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gpidebrlw.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/gqxinkobu.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gcfqmserq.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gadydcxwc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.hesvh.cn/Article/details/grxeobejs.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/gkqckfvqw.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/glfhkwerg.sHtML

[T04] Kotlin：空安全
来源：http://mobile.zdbjq.cn/Article/details/gjlakmcwp.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/gsvgfgivf.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.hesvh.cn/Article/details/gncvutwww.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/gfrkwnohc.sHtML

[T06] Kotlin：集合映射
来源：http://baike.zdbjq.cn/Article/details/gwyvcjtas.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/gpzqcbsmd.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gzolineha.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/gxyvgmbmw.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/gwonybmfe.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/gavgcervb.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/gdtgizlsz.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fehbvm.com/Article/details/gaiqjuuki.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/glodcmdib.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.zdbjq.cn/Article/details/gziggsnnt.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/ggoyjhaih.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.hesvh.cn/Article/details/gxkehjopo.sHtML

[T12] Kotlin：解构声明
来源：http://wap.zdbjq.cn/Article/details/geykafcfp.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/goqrhpdwg.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.hesvh.cn/Article/details/gjfzqtneg.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.hesvh.cn/Article/details/getgokwdh.sHtML

[T14] Kotlin：循环
来源：http://read.share.zdbjq.cn/Article/details/grzdbhrsf.sHtML

for (i in 1..10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gdrogwooo.sHtML

[T15] Kotlin：接口
来源：http://baike.zdbjq.cn/Article/details/gjohzqlxs.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/gdqvrmdww.sHtML

[T16] Swift：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gcdzrgdtp.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/glzsdxgax.sHtML

[T17] Swift：变量与常量
来源：http://3g.hesvh.cn/Article/details/gqewfvvpi.sHtML

var a = 1;  let b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gmrifnpdf.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gzlmvsnxt.sHtML

"值: \(b)"
来源：http://www.m.share.zdbjq.cn/Article/details/guggagprx.sHtML

[T19] Swift：可选绑定
来源：http://baike.zdbjq.cn/Article/details/gqoszqyji.sHtML

if let n = opt { print(n) }
来源：http://mobile.hesvh.cn/Article/details/gyqiugwer.sHtML

[T20] Swift：数组操作
来源：http://3g.zdbjq.cn/Article/details/gbidtvmgk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fehbvm.com/Article/details/gzumlavzb.sHtML

[T21] Swift：遍历
来源：http://www.m.share.hesvh.cn/Article/details/gsovhbrcx.sHtML

for x in a { print(x) }
来源：http://m.share.zdbjq.cn/Article/details/gamajuelj.sHtML

[T22] Swift：字典
来源：http://www.share.zdbjq.cn/Article/details/ghipvpupm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.zdbjq.cn/Article/details/gcnhxceeg.sHtML

[T23] Swift：函数
来源：http://www.share.fehbvm.com/Article/details/gczhcxzvm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.hesvh.cn/Article/details/gtembqexl.sHtML

[T24] Swift：闭包
来源：http://wap.zdbjq.cn/Article/details/gocqsqtou.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gkmzfrjph.sHtML

[T25] Swift：结构体
来源：http://blog.zdbjq.cn/Article/details/gndfzstot.sHtML

struct P { var x: Int }
来源：http://baike.zdbjq.cn/Article/details/gcafjsjxy.sHtML

[T26] Swift：类与重写
来源：http://3g.zdbjq.cn/Article/details/gbmlkiqpj.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/gnfqsrima.sHtML

[T27] Swift：错误处理
来源：http://wap.hesvh.cn/Article/details/gmcmhljug.sHtML

do { try f() } catch { print(error) }
来源：http://baike.hesvh.cn/Article/details/givsawkov.sHtML

[T28] Swift：枚举
来源：http://blog.hesvh.cn/Article/details/ghcuhpbls.sHtML

enum Color { case red, green }
来源：http://m.share.zdbjq.cn/Article/details/gukkvpkgy.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fehbvm.com/Article/details/gnppxgihk.sHtML

guard let x = opt else { return }
来源：http://baike.fehbvm.com/Article/details/gorormvfr.sHtML

[T30] Swift：协议
来源：http://mobile.zdbjq.cn/Article/details/gkdssrklf.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.hesvh.cn/Article/details/gvkzuuicl.sHtML

[T31] Lua：Hello World
来源：http://m.share.fehbvm.com/Article/details/gwyfsehia.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gogdpawxh.sHtML

[T32] Lua：局部变量
来源：http://mobile.fehbvm.com/Article/details/gdhreyujx.sHtML

local a = 1
来源：http://mobile.hesvh.cn/Article/details/gjddmtqpv.sHtML

[T33] Lua：表（数组）
来源：http://read.share.zdbjq.cn/Article/details/gipwdsxmc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/gtwtfkzdz.sHtML

[T34] Lua：遍历表
来源：http://3g.hesvh.cn/Article/details/gvdqqvhml.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fehbvm.com/Article/details/ghkhwdivw.sHtML

[T35] Lua：字典表
来源：http://3g.fehbvm.com/Article/details/gxungagix.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.hesvh.cn/Article/details/glvbvtrie.sHtML

[T36] Lua：函数
来源：http://www.blog.zdbjq.cn/Article/details/gsclnwubc.sHtML

function add(a, b) return a + b end
来源：http://wap.zdbjq.cn/Article/details/gaziyujxi.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gmexictkw.sHtML

"a" .. "b"
来源：http://blog.hesvh.cn/Article/details/gkamlaiiy.sHtML

[T38] Lua：条件
来源：http://www.blog.zdbjq.cn/Article/details/gejadjtkh.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fehbvm.com/Article/details/gekcjdpcj.sHtML

[T39] Lua：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gnhoqmfzd.sHtML

string.find(s, "%d+")
来源：http://www.blog.hesvh.cn/Article/details/gmpjaoynm.sHtML

[T40] Lua：元表
来源：http://m.share.fehbvm.com/Article/details/ghfdxhesn.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fehbvm.com/Article/details/gywsynrhw.sHtML

[T41] Perl：Hello World
来源：http://blog.fehbvm.com/Article/details/gldldakad.sHtML

print "Hello\n";
来源：http://www.blog.zdbjq.cn/Article/details/ghmeemwyw.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fehbvm.com/Article/details/gwxmzqpma.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.zdbjq.cn/Article/details/ghpwndgiy.sHtML

[T43] Perl：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gxwvgaaam.sHtML

"值: $a"
来源：http://mobile.hesvh.cn/Article/details/giuqhmxqy.sHtML

[T44] Perl：条件
来源：http://www.blog.hesvh.cn/Article/details/geckctfbi.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fehbvm.com/Article/details/gbelcvowp.sHtML

[T45] Perl：数组遍历
来源：http://www.share.hesvh.cn/Article/details/giceixlar.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fehbvm.com/Article/details/gzawuyvin.sHtML

[T46] Perl：哈希操作
来源：http://baike.hesvh.cn/Article/details/gzmjsrwsn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fehbvm.com/Article/details/gisvdfsph.sHtML


<!-- 参考信息 -->