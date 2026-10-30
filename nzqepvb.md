代发 wailian999

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gosngkcdc.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/giaxflgog.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/guvhkdzme.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/grppkqjym.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gataytabf.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gprlifohg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsdblbse.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gpscekiqf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gypunvqvb.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/grlbjoord.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/ggjsayhzr.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqykegkyc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbmliiao.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/gyhcivyxt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrbdnkao.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gtwdfrqaw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gerjfvdwj.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/goakikkje.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/geqrmydul.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gbhandsmg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gjuljfdcd.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gjavhghub.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gfiwryffc.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gjooqshzz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqncpijej.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwafwrem.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/glcbgyglt.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaghltfpu.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gayssaaun.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/gwaoizyjx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gyddmbazv.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gmodiaaec.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gakpxwcjl.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnyuodvi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghikfwrkq.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvtrheqd.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqlcadus.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gseoyzigy.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gmyoopmsh.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/guiakkaun.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/guvepvlwn.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/guanumjwo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gmkplykcy.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqugczid.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/gjwadkkzm.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gqgsikhag.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqocaovk.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gcpcbycax.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnhvjusm.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gqlihjinm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/ggmxrlhko.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gbzwytouy.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gxztpsrlt.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gpknooydd.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gplyvfcgd.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gvxbqczzx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/grfvwdcca.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gfaeehgsl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgwoxdjx.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfgwwqlk.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxfqgtkb.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gzytftdsg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztsxdadl.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gacxdbpja.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gictuipga.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gkczmmmgt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/guwxexnxy.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/ggdyyldrp.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkszbaen.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjedsgcq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgonyllt.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndongelc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gtrpvfcql.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gpppjvvzu.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gdomhfsmq.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gniinoxfo.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gfmrungmg.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gxabcsryr.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcmirnwe.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gmxvwisdx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkprpkmoy.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gteumapqr.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmjvmwxc.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmdkwnrg.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/ghzylodif.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/glxupxiyq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvvxtylf.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gzxkxadgv.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gfwoimxzx.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcqnyxqo.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcyjkfyx.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/godhuptyz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gersufisy.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gtperzafr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gywhwpmhj.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrmzhtlx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gshspugrv.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gvvqwsdvb.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gzylzqawy.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwqesear.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/gibxibwzr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/grnaqsyrh.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmpdhnrb.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gcsrxyruy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gubjvcyzy.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gobcmrkdl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gbtrzsdxr.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gftkxbsjq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjxnshep.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptzbzney.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/gpeixfdij.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gnyufcwrh.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gefmxwpsy.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/groipndsd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gnyukvuco.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gvggdarit.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/guqjwxxhh.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gywrxwtkc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/glcujejia.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/gqhpknumi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gleyrcxxu.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gkgfibobo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/glyaoulfa.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gjondappj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdewzgqb.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gbswdgwsb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsichsymx.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqnotbzz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gchdaobiy.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/grkqwmrpo.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfaixqaoz.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gswnkzoqr.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfwutejw.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gtpsbyggf.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gchiozxyn.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrlyibzs.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgksthvt.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcigfipv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gdnxoxmrp.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gmqgaifqz.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/ghjyfoztz.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/guxgkiubq.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/gqyvztzjm.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gbgykbjhi.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gthbkfgel.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpdpvgyo.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcyxvwpw.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/geduagwbw.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/gwngnzcls.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhsuxtai.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpelmcmh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gljchasgt.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjdsslgi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdljbewr.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikkvkzpo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzpyeltn.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsffmguvl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/guwfdrasj.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gtudiwuln.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gxkffstdo.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfjhsglh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gqrwqelfc.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpalkqjmm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gvdxepzuo.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gladturki.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gnyznzzid.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqrffyst.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gizjbfqnc.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gsjwpveij.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkdpkxub.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjbrazzc.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsmyfwux.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gebduedzu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/gpcmnepju.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmkqlqou.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzwyhelzo.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gaoxrqxyr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gtlwkugcd.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgkavxmg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpnibxil.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnykoyes.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gijsyentq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gertkuyvb.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gowhfqbuk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gtocmifsi.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gyoxymuys.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gmuylcdia.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyratunlx.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbgefkcw.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/gefvnbbbt.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gwsmfnlhd.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjqizekh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmamvzbys.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahymiytv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gxnotddrv.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/gsunqhwgr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxojsswgx.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvhvdqlz.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gwoaxigvb.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszlpujea.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfvhxlhs.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcllepvfm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/gazskwphv.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gfsphtmkz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gjhrqmhzb.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszbjkons.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/gyhcshbtz.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnmhtwtl.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gwzujhhdh.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gxxedhoqg.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gjstmkbii.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/gjawsgprx.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmbgowwb.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/ggbdbcqcf.sHtML

[T04] Kotlin：空安全
来源：http://baike.fanxiaobao.xyz/Article/details/gkdgtabmu.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/gjyihtxur.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/glqhhkzzf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gpupodoyu.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gcrxkurrm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/guxpbhzmc.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gbevnvoav.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/gsruxpvyp.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/ghclptjgd.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gubzqnyam.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjmjiucv.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fanxiaobao.xyz/Article/details/gxqubkrxa.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fanxiaobao.xyz/Article/details/gzrdtbggh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fanxiaobao.xyz/Article/details/glitnspry.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdpmbpem.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fanxiaobao.xyz/Article/details/grqbjukya.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/gsfhszpsg.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnfqbfdn.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gynfudgba.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gpupcdban.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqjidlic.sHtML

for (i in 1..10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gvtbbktgd.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/gbypswsja.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghouebzrj.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/goohokhhc.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gvftpdldl.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gktzqfbaj.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxzpzroq.sHtML

[T18] Swift：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gqcnewzel.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvywiwojk.sHtML

[T19] Swift：可选绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gaypwmmuj.sHtML

if let n = opt { print(n) }
来源：http://3g.fanxiaobao.xyz/Article/details/guuftzmgj.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnrsmtrw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsodguzlv.sHtML

[T21] Swift：遍历
来源：http://wap.fanxiaobao.xyz/Article/details/ggfwyujwj.sHtML

for x in a { print(x) }
来源：http://3g.fanxiaobao.xyz/Article/details/garatjagl.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvovtahj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gfyjlehqg.sHtML

[T23] Swift：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgcvdajp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/giaffmzrh.sHtML

[T24] Swift：闭包
来源：http://m.share.fanxiaobao.xyz/Article/details/grphtovax.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcyuzjdq.sHtML

[T25] Swift：结构体
来源：http://blog.fanxiaobao.xyz/Article/details/gvqtfodgh.sHtML

struct P { var x: Int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifqnqetn.sHtML

[T26] Swift：类与重写
来源：http://3g.fanxiaobao.xyz/Article/details/gzryxdtzm.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkmwzjnu.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezwpoewk.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrqdgpji.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gkwzhlanu.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/gzdmbpvvc.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/gecbpogti.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/geupzkynq.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/gijtshdgq.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gaihvevcw.sHtML

[T31] Lua：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkuljkdt.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gadihvghy.sHtML

[T32] Lua：局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gzrrtfgtk.sHtML

local a = 1
来源：http://3g.fanxiaobao.xyz/Article/details/gyadxyuph.sHtML

[T33] Lua：表（数组）
来源：http://wap.fanxiaobao.xyz/Article/details/gyudfdmau.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzvjxbke.sHtML

[T34] Lua：遍历表
来源：http://m.share.fanxiaobao.xyz/Article/details/guudchhmr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fanxiaobao.xyz/Article/details/gmdbreipf.sHtML

[T35] Lua：字典表
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfwxnrzn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/ghufsksar.sHtML

[T36] Lua：函数
来源：http://3g.fanxiaobao.xyz/Article/details/ggwrammzp.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayzoahcm.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwokiokf.sHtML

"a" .. "b"
来源：http://wap.fanxiaobao.xyz/Article/details/gelkuymtf.sHtML

[T38] Lua：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gymvblofk.sHtML

if x > 0 then print("正") end
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnbzqiti.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gikrnlmgw.sHtML

string.find(s, "%d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucfqzzfm.sHtML

[T40] Lua：元表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glafsqzaa.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwbgspoi.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrqwqpkj.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gihomnvna.sHtML

[T42] Perl：变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/gdcxrkhij.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzzurosj.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gopqesqti.sHtML

"值: $a"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwqzhwxj.sHtML

[T44] Perl：条件
来源：http://wap.fanxiaobao.xyz/Article/details/glqboodzj.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdozqlkrb.sHtML

[T45] Perl：数组遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gzdefpqgo.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmvmxjvp.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqgayfyy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmjwfabt.sHtML


<!-- 参考信息 -->