代发 wailian999

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gytqulcna.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxseigtbq.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpkffrvp.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gzlksxmwt.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcsckejq.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gecjfneza.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkoajnacv.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gdulxjexi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gngxkpapp.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gormjrntg.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/grlbxmhdw.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrfwszaj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/grpjpdotu.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gaikadfaq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gkgzrhsyt.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvenmumeg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdudcynm.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsutojmua.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gmmmivnrw.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjdhqeno.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/ghevffyoo.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkpzhkix.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/ghqsfdnnp.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnfnnzxt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gpmnhtvkf.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gmzfewgdo.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbfsxqcp.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcriazkx.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gsspxlrmh.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbhgmvhy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxkuoryh.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gdxxsewro.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gqasmxpdd.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gdegfclnz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqelimnq.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigdntiig.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbmhntsi.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxagabbj.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gojlxvdet.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gwnegzjjp.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlucpgyr.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gbrtulfhe.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnmktxox.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gjnlgahum.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gajzxrecg.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqkmgbut.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gndebxvqs.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpzumjnm.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/glzjionpo.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gfmdewmis.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gizvqpxln.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwccpeci.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gfihnuzqx.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gsdqtqimv.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrbyqaqi.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifbtmbxn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gaulunsji.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfhjgatc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gddtwbfbh.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzdecqfz.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaecevnak.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gdinsqwtf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gtjvtbfhp.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfkihcii.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gslkhwutq.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gbpxogwcl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gpalqwndg.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gngulgvyc.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/ghckvhyts.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrhhhybf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gawbnjtto.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gwnurrihh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/ghkmbjbjx.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/gnoszwppc.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/ggkoslcik.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbqhuuwg.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdhlulsi.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gwyacaeex.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisrtqgib.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gitaqxotz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/gydynozew.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gwbhgmkrh.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbiyqvxn.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/ghbdfukds.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbqtoagg.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/ggeilxtdh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/govkvrvrl.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gbikbjywq.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajxfdsfu.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gboktrqns.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/galxsvsmx.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmurntqq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gquukyiya.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxmfdahk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbaibgpdg.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/geibmxfps.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvtmwaww.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqdingla.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgsoonwx.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gkjnzmkfx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjeiwnth.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhvssdkv.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvzbrwgf.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gtkievyxg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gachzvzas.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemtyayhg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlrqakql.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gpcwktitk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gtwgcgxig.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhjxoxko.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/ghwnnsaii.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/ggxykmcbg.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxhntsco.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/ggegokyif.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gkglztkjr.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gfuhgyfqk.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/gscioiqar.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gwchiszte.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gwlrppncj.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gnhrvfkhz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gavgxeivq.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/gbiqsmrhi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/godpgoaln.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gqeavzweu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwsgofwf.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gihmuspwu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhrkcdai.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxnlyrwa.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/grmtgxfcx.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudrgmikn.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gfsgwxxca.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpslmygg.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbhxxovg.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/getgnpuiq.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gynloulpy.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gimonygph.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsjmzsbc.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgpgbnln.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqdykhdh.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gvshjqbtm.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvpbvwvy.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gnrymawxl.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgxixrzc.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gutbygdcc.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/goeycnocj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/geclrvfsz.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gfioplmmw.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncjqfjwu.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gzoddqihg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvydhspq.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/gofnhigqb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghqimqyqu.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gbemsajuy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/guamkahiz.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskznkfgy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdiyzklop.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/gfabxxmiu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggccxotul.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnrrnofl.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gcomtskse.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/gbkirtvyb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gpgkjkkvr.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozjppxpv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpouzxsj.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofusyxky.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gidgrxlfd.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnzkxdll.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gpojqqitd.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhxnomgs.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjuhapksm.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfajksrq.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhlzbhht.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gryddzqao.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/gnrzihscx.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvzmdakg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnpzygys.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gjltjuhin.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gaczxefnl.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gckdzcvrk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/grvojptfv.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyndhknqp.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gktyfboux.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/guftjfbtp.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gioiiaxvd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjececfyn.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/galsplveg.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihqwmjzu.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjzcwbeq.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/goujstoxo.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgzlmhfp.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbqqgwrp.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gmkknowbk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjznfmmdo.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gnynizbtv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkzmmsxe.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gttpvqaud.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geojnpfgt.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmcwuonj.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkteviyr.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gasxawijd.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gnevyzmoi.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyikjlnef.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtyranpd.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxopwdoo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gffgjaouf.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/goljodmyy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/gylbynrcm.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gbsdxbmcj.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmnmxmoh.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/glvselsoz.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gvoyywblz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/gswyidfwn.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhivkuby.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gajsbhpvs.sHtML

[T04] Kotlin：空安全
来源：http://baike.fanxiaobao.xyz/Article/details/gnbpwxryj.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gihigalof.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gryxikaqp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcozlxot.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gahyqscsq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgvtcsmz.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/goelpbszn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/guaivbrfv.sHtML

[T08] Kotlin：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gkjzcldjs.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gmxnlxwdc.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gyldruoxw.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/gelqckomo.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/glaoundfc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fanxiaobao.xyz/Article/details/goiqtrutx.sHtML

[T11] Kotlin：协程
来源：http://mobile.fanxiaobao.xyz/Article/details/gipanffyu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fanxiaobao.xyz/Article/details/gixpfqcvi.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/grgsspebk.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtjmvfry.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gjqgegyel.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gibtdmvcb.sHtML

[T14] Kotlin：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxztsfor.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtuxantdu.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjicdqfzl.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjfddamp.sHtML

[T16] Swift：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/ggtevrjfm.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/glkbtnwuj.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxdwvjxb.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gfirgtowo.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmfiqqyo.sHtML

"值: \(b)"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqthclmk.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpgmnndb.sHtML

if let n = opt { print(n) }
来源：http://blog.fanxiaobao.xyz/Article/details/gktanmdml.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/ghtvkvpns.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsngkddh.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gxdmbvoco.sHtML

for x in a { print(x) }
来源：http://3g.fanxiaobao.xyz/Article/details/gyogmldsd.sHtML

[T22] Swift：字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gzefycfon.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gfbujwkxu.sHtML

[T23] Swift：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gabsyscim.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gwfksspiz.sHtML

[T24] Swift：闭包
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmxqmvya.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gvvjlphqe.sHtML

[T25] Swift：结构体
来源：http://3g.fanxiaobao.xyz/Article/details/glojtkxej.sHtML

struct P { var x: Int }
来源：http://www.share.fanxiaobao.xyz/Article/details/gptqwtgcd.sHtML

[T26] Swift：类与重写
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwscbtra.sHtML

class A: Base { override func f() {} }
来源：http://wap.fanxiaobao.xyz/Article/details/ghjrpazzy.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnqfeala.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fanxiaobao.xyz/Article/details/ggadmjiin.sHtML

[T28] Swift：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gwmgmvrme.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/gwhswkosy.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/gixfshrfh.sHtML

guard let x = opt else { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtaypczhg.sHtML

[T30] Swift：协议
来源：http://wap.fanxiaobao.xyz/Article/details/gilroaugw.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/glqgkqkdv.sHtML

[T31] Lua：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gbplzmjif.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gazcclddy.sHtML

[T32] Lua：局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gflzgelyx.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/gplbflzsi.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fanxiaobao.xyz/Article/details/gqyrvetmj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fanxiaobao.xyz/Article/details/gcelfuhmr.sHtML

[T34] Lua：遍历表
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnzwunic.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fanxiaobao.xyz/Article/details/gabtvityy.sHtML

[T35] Lua：字典表
来源：http://wap.fanxiaobao.xyz/Article/details/goevaumts.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/goshkiuqg.sHtML

[T36] Lua：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/guayfrlmh.sHtML

function add(a, b) return a + b end
来源：http://baike.fanxiaobao.xyz/Article/details/gxxxivkwv.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvmvcsie.sHtML

"a" .. "b"
来源：http://3g.fanxiaobao.xyz/Article/details/gtnpjnwlc.sHtML

[T38] Lua：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdirkvouy.sHtML

if x > 0 then print("正") end
来源：http://3g.fanxiaobao.xyz/Article/details/ggnebdmxq.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goanqbckg.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrrjfkye.sHtML

[T40] Lua：元表
来源：http://wap.fanxiaobao.xyz/Article/details/gfmlysuhi.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fanxiaobao.xyz/Article/details/ggudbeeff.sHtML

[T41] Perl：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gidsbjxda.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gkohjfinn.sHtML

[T42] Perl：变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/govplxrbn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxblucmy.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqzxgeor.sHtML

"值: $a"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnanbvtay.sHtML

[T44] Perl：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gcotizoaq.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gelcsfhcg.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpghkdgt.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/glhxslvik.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlpkjkeo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkgrtrgzs.sHtML


<!-- 参考信息 -->