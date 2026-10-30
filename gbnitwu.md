代发 wailian999

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gnpjowunj.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gtupuicut.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxvfbylc.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gaflylmqg.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gttlkfvlw.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrgikpqc.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxuamcnhw.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gctmmidwc.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/ghaoacogp.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbxlsgov.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gbuezmixc.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/glbwkbouf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/glnqavwta.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gafjijmye.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnghwcio.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gppuqesja.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gzkbsybij.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsojlfgdw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmqruvfx.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/ghwcbfabw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gtddtifiq.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gkhbmnmev.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gzdfaoyjz.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgdviaqo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfhosorg.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gxsmdyvxb.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqinzyiac.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gjupallks.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gbsuvrtfe.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gjgkdyvda.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gkwnwyzjq.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdxijjwr.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxlcvoxl.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gqghcvmxg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gllqyxoan.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvwfhipr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gcpyboxgp.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gdlxupbgo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxqpmabk.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcjbgapa.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxtbbhyz.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/grtkmkyzi.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwtvmvda.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpkddjgl.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsfrbdjd.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gparfedrt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gbdqfqjdk.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gcamujsof.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gxzjwtsor.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkrwynef.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/guxfepbox.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkavpgocc.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gzygnccso.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gewjmkzaa.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gctkdises.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpqkaxvg.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gggopmhka.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gojluhaqj.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnupiensb.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gpucwhzmb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gdqsbuuwk.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndiitvuq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gpxvkrscx.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcispzyf.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gjushersd.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsrjbgte.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwkbbyqf.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gyayvfcuh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsuutsjb.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdudocqaf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwhinpcy.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzddeedn.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/glkrmgumw.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gogjcaxdm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzsdslao.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geexlqals.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlwvguso.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gkikfxwgt.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/gwsjkyemv.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqpmgmef.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/ggisczprd.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhnlohyy.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdrunxjr.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsfljghu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/galhbpefo.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/giwrecbqr.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaylbgrew.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gdgqohbxk.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqqxtmvh.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyuwukrt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gquykqxlx.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmdeoexc.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/glofjjbro.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gjopjzzdp.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gmgxkglru.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvrfbeop.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/ggwhebjsk.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/gwthxwhhp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtpdwmxv.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gqbcyxxlf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxbosmha.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gpdayauye.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gjjfdktny.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gwznreumf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/grcyzdxmx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gfwkqzolk.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/giuybqswf.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gyzksizel.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/glbsbzaqg.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/guynogcyr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gflpbajsm.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gqjphnvzg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/grgkibrid.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzlepxfc.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/gahtgehet.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gyutcqvmu.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/ggejkzvcp.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gqnnjffqz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gdhdcnemi.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/ghwmeajin.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gzehqsjmn.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gknyuupdk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gduvnduei.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtkwvodq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gchaedtaf.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgkcpbsm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxutepqny.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gthfdomdv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwicrvtk.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/grelottck.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gzmggeizw.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekxcghuv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzecgfuom.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gblquifwe.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gniqyncum.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gjxmgfzkr.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gswwiyxqq.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gqniapdfu.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gmekiyqjb.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqnipevl.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gxsqlvgrm.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/grayihpfc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guozzvlka.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzjtufpi.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrdcqdig.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/geelutpby.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwzeyqeo.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gfsswvvlm.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gcjljsjgp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphratmjn.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlepzdyr.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gztgfsvuf.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gmhinzjlz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gopmvjyzr.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgnqrwwu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzfpxfgns.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhqtckgw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gtxqbcjni.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpddfkyj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gklszvolp.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gmeispcot.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkanszmxr.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gvingrlgr.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/genstymfg.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gvuovaaks.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzjcgciy.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqguzkuj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/geemhmofc.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gzneiduhv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrhrpbnb.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/ggubwioxv.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gndukwedx.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gzmmbxsss.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/guxdbckkt.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtzqqozk.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gnzznwzht.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gszqtkrcx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gzuwgtito.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gvilqjheb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gstftjadm.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwuiyozha.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gztwbshus.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/golmdrbfm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/gasimwkvy.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmxjyukm.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/geetmbttc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gclzqfejk.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gzycubing.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gfgkvwpcl.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gotkfcglb.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gmxcqpvoi.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gtotifosg.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/geigvsbgv.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gmkvbqzua.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/gefvqxdtj.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gibuivyxj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhjexmre.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gnhhfpslj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsncpgfkj.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/gqjykrpzy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/glmvbobyr.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gatdoikqm.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gcehcjvai.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gofawqdrx.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gdycxjsrp.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gxgheqqeq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/gesmypzhl.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/guyqomfjq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gilpbcoue.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsgjipeq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gxyotyuqc.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gryvioewm.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gfoecnxgy.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gxczjruqf.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzcjugxm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/gydljwfey.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/giebkmtpd.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gpzurjqix.sHtML

[T04] Kotlin：空安全
来源：http://baike.fanxiaobao.xyz/Article/details/gymtbnrpd.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkvobego.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpijpxbur.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/gztnkhbgn.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkzwphbb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gplhcyahq.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gfgpzvyql.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghivkvpjq.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnuqfxpy.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gilgredtn.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbrxtdwi.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwechyre.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gzenbwotm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gaekrdyvj.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/gjnkcrisf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fanxiaobao.xyz/Article/details/gnkaumpuo.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/glhzlvbot.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmrivrbf.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/ggllzhjyt.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkojcnaxa.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gomimyrwl.sHtML

for (i in 1..10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gxaogtiww.sHtML

[T15] Kotlin：接口
来源：http://wap.fanxiaobao.xyz/Article/details/gzzfcuuot.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyyzbguca.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gszzyufgt.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gafxztcsi.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudhwveom.sHtML

var a = 1;  let b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrymygry.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gjpvhbjjm.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/gumcguqrm.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/garnqksdw.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gplnkijju.sHtML

[T20] Swift：数组操作
来源：http://3g.fanxiaobao.xyz/Article/details/gcdzwwjka.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gwmuqtupt.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsiozsgm.sHtML

for x in a { print(x) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdyxrmte.sHtML

[T22] Swift：字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrjxtreo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gyeaoodqb.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gvhlxgezx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfejnpof.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gvbhclrou.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gsavvyqso.sHtML

[T25] Swift：结构体
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqeycfei.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/gzumljvsc.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/gipvemyil.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/glawwuhtg.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopvhpqmb.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtynottfz.sHtML

[T28] Swift：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggswxvghj.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxauipcvj.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/grtprirdo.sHtML

guard let x = opt else { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmacxpsq.sHtML

[T30] Swift：协议
来源：http://baike.fanxiaobao.xyz/Article/details/gcwgiephk.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fanxiaobao.xyz/Article/details/ghmcreehy.sHtML

[T31] Lua：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gfaaiuuwx.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtltwifx.sHtML

[T32] Lua：局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/grzwqsaiy.sHtML

local a = 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcgtnvgz.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfknshwfy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfxpgjwh.sHtML

[T34] Lua：遍历表
来源：http://mobile.fanxiaobao.xyz/Article/details/gxowagavw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fanxiaobao.xyz/Article/details/gusarycbb.sHtML

[T35] Lua：字典表
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgjqldwg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqvxdmav.sHtML

[T36] Lua：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gamjrlrjd.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmcjvfth.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gxyiiyign.sHtML

"a" .. "b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgmwsfsx.sHtML

[T38] Lua：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjbvvrli.sHtML

if x > 0 then print("正") end
来源：http://blog.fanxiaobao.xyz/Article/details/gmqyudmqj.sHtML

[T39] Lua：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gnurmilrc.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfypzcbz.sHtML

[T40] Lua：元表
来源：http://wap.fanxiaobao.xyz/Article/details/grsabbkhr.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fanxiaobao.xyz/Article/details/grazycbjo.sHtML

[T41] Perl：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmwihusq.sHtML

print "Hello\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gqmenzgcs.sHtML

[T42] Perl：变量类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjcriinh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gssszmwap.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfuqpwlij.sHtML

"值: $a"
来源：http://wap.fanxiaobao.xyz/Article/details/guzeglgvo.sHtML

[T44] Perl：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gyitdcjbt.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gotzzldrj.sHtML


<!-- 参考信息 -->