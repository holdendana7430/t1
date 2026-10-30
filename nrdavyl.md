代发 wailian999

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gttbrldvd.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/gazbxnjtp.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrhwsmku.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/getndttwb.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gulytopqx.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfieffna.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemrckdxz.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/grrjwtcnz.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gduazkqej.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gnzwdajxg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gnevshadp.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/glcyuvbjf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpyvjxkl.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gbiyrdisa.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gudrsxjhz.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzwpmjgo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gzlicumrl.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlrfubsn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwxqjnrb.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlwiqcma.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxhrqcyi.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gxbfmonwe.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gkpakhgbw.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrktrpcg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdivaspq.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gipnfkqqq.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmiznvfle.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gszxwzogt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gyawuhobh.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gsyiqiqig.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/grcgzaddz.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gbazfxwwv.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/grjtvgcmc.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gjutwfqtf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/grwsewscl.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gastyjdcg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/ghrocktyc.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/glkpzjvvv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpcwktcx.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gugocfomy.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrmlekyj.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gqbrzzbmn.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatifxgjz.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnijcowy.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavfwkjtu.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gcwphbxlp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gspvjzezr.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtosvddi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/ggaxtequk.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdfcrnmh.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gdyxgzhew.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gzvyrvydq.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxztimunf.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglymnwuq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgdwhhrd.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrstoeon.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gugrhpdqs.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gsxsufhnm.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvgdzczi.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/glzelrzsx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhkphkbm.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/gorhmgrlw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gwuxcgyrk.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxtwmyuz.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gsexazyqq.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gciydlpiu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gephjdutc.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gxtdeqrla.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gpunkspzk.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbifejyb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsmwueir.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gbxinrzuv.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/guqgdimwy.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqpnrzde.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gppopdwvx.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gbwyrjlfl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gqeddvadc.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfowxhvkp.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gztwmzeug.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gqoivudkq.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhnfnbux.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/glomhahla.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gewcjdffl.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gomoshtgz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfoqujcy.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gktgsxtqb.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gospewogj.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwoskgyc.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkylwpcee.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdnucaqo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/ggbhijgsa.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghitrukzh.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gwqqinvov.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gzfbrlivm.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gotynhpew.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/govgwtwrw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gylfwwzsx.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbismgnt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbawjvzm.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gkilvgfgd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/goecaigcg.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gyhdwpozj.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gjinbnddy.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gcvnmfolj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gpcoxxcnv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gshymealk.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrhhmonn.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guouixtdz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcazcukho.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/guuufpqai.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gyuevgeqw.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/guxipugub.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/geqnzcpjv.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gskpwwnfx.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/guytoyibe.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/geqbzfyug.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfoauobg.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcntzdej.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzuahmnt.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjvzscqa.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gqxaevyic.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gvluikvaj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/guqnkcbke.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvhmnuxp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gcfsmpzex.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gjieybmqd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/geactqbmz.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gnhdyzmbe.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/guaoaourb.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnkzdwgy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/ghghjlexx.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gkzjzofcz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyuabmygu.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/genrfkwvb.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgbbckho.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmwvwaki.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsemnufl.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhzqaiym.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gqncqjixh.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gzednwznd.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gurgeyxoh.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjahngjvu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmyxlztwn.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/goyamyodh.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgimvjvg.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gqaxejmpn.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqhnwvfu.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/goohllxcw.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpjcimct.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpqyzbwn.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgfdaoqc.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gnnuhqsne.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/glcpavtua.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/golvxfggb.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqmndnsa.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/geclebwwz.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gibsdxvzi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gysdxfibw.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazurhdwj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gofinmked.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbuucmhzd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gidieovpo.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/gkmwowrej.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gqflxzeuv.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gezxfcado.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gyvzkusfc.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gcuzrbwkt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/ghgykgovy.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcoysujhq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gfongazaj.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaznzheaq.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gicpaytzq.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gkegnzyoo.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/godqsjpwd.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/glgcrefkj.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gstzqedaf.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjugonsi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gixbkcjfm.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/gfcmssqsa.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqqwhant.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gnvqtvray.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdoydphq.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gytzrujgf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnndysdh.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gvpakjrpt.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/glejgdxmi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzdwbmrz.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrdzqpkq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gibwpurtn.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gccnuttke.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyycztpnc.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/gviwuffzh.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gznxuwrvn.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/gynwxeupt.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gcziywpwn.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnxlkjfq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzccijnp.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqszdhid.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsjzocqw.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gtmpsqpib.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/glwxvldfc.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gokskwoiu.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/grfwwkdfi.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfdpvgjg.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwmkrgzm.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/giqulslvy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqiguizf.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhibtryc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gonharzob.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gikwsjila.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggselqwdw.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwevsclo.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqpqjsbj.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/glsvjrjen.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gfapwlbml.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/gapjyjhis.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvenoubsh.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gosgyakea.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/gsepbuxab.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gksppfhar.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuphouem.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/ganrlshqn.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gogsjdkms.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glywlvekd.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gkgwosxfe.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbosmvsf.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gioemethu.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzduypikb.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fanxiaobao.xyz/Article/details/gzfzibfah.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/gspgcthsb.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/ghcadpisl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gczawqlhx.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/gyhdtnsis.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmhdyqqg.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtxypnun.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpttssuts.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gsvhlyhrv.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhnirpfz.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gmwlyovbp.sHtML

for (i in 1..10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gnshnpbkq.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/gnetnmmlg.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gbbbrwbpn.sHtML

[T16] Swift：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gznxhnaql.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkhtsdaz.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrurshqn.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdilqfyda.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdxlhink.sHtML

"值: \(b)"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbnhzggf.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnepsoqld.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgwcfbzd.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/gzovzilcj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guyooquho.sHtML

[T21] Swift：遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcgevmro.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/gxctidhjj.sHtML

[T22] Swift：字典
来源：http://blog.fanxiaobao.xyz/Article/details/ghgljjcgn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gsaoennxq.sHtML

[T23] Swift：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjuyktbuo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gtkuupxhc.sHtML

[T24] Swift：闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/gofdgnjad.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gepdyxbir.sHtML

[T25] Swift：结构体
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbaabsap.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbngisduj.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrwqoare.sHtML

class A: Base { override func f() {} }
来源：http://wap.fanxiaobao.xyz/Article/details/gqmcnxjsv.sHtML

[T27] Swift：错误处理
来源：http://3g.fanxiaobao.xyz/Article/details/gzuojmftk.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fanxiaobao.xyz/Article/details/gwbivyhyt.sHtML

[T28] Swift：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gwpuiubhl.sHtML

enum Color { case red, green }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqqcpmfr.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/gorsrpvbv.sHtML

guard let x = opt else { return }
来源：http://blog.fanxiaobao.xyz/Article/details/gluwadafc.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/gnaxytqfl.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohmpzvho.sHtML

[T31] Lua：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gxrryxnbd.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gagssskhj.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfnfmhcq.sHtML

local a = 1
来源：http://m.share.fanxiaobao.xyz/Article/details/goqdlpeio.sHtML

[T33] Lua：表（数组）
来源：http://baike.fanxiaobao.xyz/Article/details/gujbijlpi.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fanxiaobao.xyz/Article/details/gklpnhtnz.sHtML

[T34] Lua：遍历表
来源：http://baike.fanxiaobao.xyz/Article/details/goktrfkiz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fanxiaobao.xyz/Article/details/gdktbveki.sHtML

[T35] Lua：字典表
来源：http://blog.fanxiaobao.xyz/Article/details/gvesjyhdk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gqccftsdb.sHtML

[T36] Lua：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghulktus.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/gsscglonq.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbxelrij.sHtML

"a" .. "b"
来源：http://3g.fanxiaobao.xyz/Article/details/guaqbeksu.sHtML

[T38] Lua：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gaqmbraty.sHtML

if x > 0 then print("正") end
来源：http://3g.fanxiaobao.xyz/Article/details/gmsemcpui.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrlbsvye.sHtML

string.find(s, "%d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gfmjsbxvr.sHtML

[T40] Lua：元表
来源：http://baike.fanxiaobao.xyz/Article/details/gjmluayar.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfisnugyb.sHtML

[T41] Perl：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gbztxmqpn.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbcxgdxb.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawqnkwjz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrjzrits.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhsxbvkl.sHtML

"值: $a"
来源：http://blog.fanxiaobao.xyz/Article/details/gftkytgzi.sHtML

[T44] Perl：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxdolhbh.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmazpykma.sHtML


<!-- 参考信息 -->