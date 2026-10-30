代发 wailian999

cmd > out.log 2>&1
来源：http://mobile.hesvh.cn/Article/details/gfpvwaala.sHtML

[R40] 追加写日志
来源：http://baike.fehbvm.com/Article/details/gtqznwixi.sHtML

echo "log" >> out.log
来源：http://wap.fehbvm.com/Article/details/gbygssviv.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gqjtwodfy.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/gzhdtunpx.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/gkyupfgbp.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/gwauyumku.sHtML

[R43] 按名字查找文件
来源：http://blog.fehbvm.com/Article/details/gyjujscnl.sHtML

find . -name "*.log" -type f
来源：http://read.share.fehbvm.com/Article/details/gzgjulite.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/gfpajoosu.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/gadoagghd.sHtML

[R45] 批量删除
来源：http://www.blog.zdbjq.cn/Article/details/gebmahyla.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.hesvh.cn/Article/details/gqngzjmma.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/glyblbmci.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/gvbhkuyrk.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/gximjrrkm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.hesvh.cn/Article/details/gzrmwtzjx.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/grmeihmgo.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/geuyvtfqx.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/gfzrfnhnd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.zdbjq.cn/Article/details/gsyhdofhj.sHtML

[R50] awk 求和
来源：http://blog.fehbvm.com/Article/details/gstsopipb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gqksxoavg.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/ganxzytjr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.zdbjq.cn/Article/details/gtacdgfae.sHtML

[R52] 统计行数
来源：http://blog.hesvh.cn/Article/details/gfarwdmrk.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/gzcaxiznb.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fehbvm.com/Article/details/ggvcftwpl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/gqucutyhd.sHtML

[R54] 比较两个文件
来源：http://read.share.hesvh.cn/Article/details/gkdpskbec.sHtML

diff a.txt b.txt
来源：http://wap.zdbjq.cn/Article/details/gplqyualg.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/gzhpfpkug.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/gohhcvdjc.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/gkqqywxyx.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/gwzvcyajw.sHtML

[R57] 远程执行命令
来源：http://www.blog.fehbvm.com/Article/details/gruwpgqke.sHtML

ssh user@host 'uptime'
来源：http://www.blog.hesvh.cn/Article/details/gthvtufwt.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/gelcvzcys.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.zdbjq.cn/Article/details/gfflfzvxw.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gtgqnibea.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gjvktxntd.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gupsgehwj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/grrhifetn.sHtML

[R61] 磁盘占用
来源：http://m.share.fehbvm.com/Article/details/gvvpbxgqy.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/gvxhhmltx.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/gmnwpenyo.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.zdbjq.cn/Article/details/gnaiqvvmo.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/ghsfwnaom.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/gizzlbmft.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/gistniplt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.hesvh.cn/Article/details/gtolnlufc.sHtML

[R65] 查看端口占用
来源：http://mobile.hesvh.cn/Article/details/gvjfvdsbi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fehbvm.com/Article/details/gkztkxonr.sHtML

[R66] 定时任务
来源：http://read.share.fehbvm.com/Article/details/gpyemkqhn.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/glqhoqhvp.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/gxhlkbbee.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/gqemfqqjh.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.hesvh.cn/Article/details/geimvplal.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/gghuuwsqy.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fehbvm.com/Article/details/gjqjyclni.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.zdbjq.cn/Article/details/goxhorueu.sHtML

[R70] 时间戳与互转
来源：http://3g.hesvh.cn/Article/details/gxicjxfkk.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/glvdxoksw.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gickkmbii.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/gfmenribf.sHtML

[R72] 等待端口就绪
来源：http://3g.hesvh.cn/Article/details/gkckrbdsf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gcidcxrbh.sHtML

[R73] 分割大日志
来源：http://wap.fehbvm.com/Article/details/gfkjlefvr.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/gxsmuhuco.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/gtsvguudw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fehbvm.com/Article/details/gmelxmcbb.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/gqzefrcfd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.zdbjq.cn/Article/details/gipcdplbk.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/gwwzenkrs.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gvfixsvow.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/gvkcjcxzk.sHtML

read -rp "请输入: " ans
来源：http://mobile.fehbvm.com/Article/details/gklewblfg.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/ggwvpyusu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.zdbjq.cn/Article/details/ggarwissi.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fehbvm.com/Article/details/gkngudzib.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.hesvh.cn/Article/details/gqbxcqisc.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.hesvh.cn/Article/details/gvquthslx.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/giruagdxo.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqyyrglcg.sHtML

S. C / C++ 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gznpyswzg.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjsqceojs.sHtML

[S01] C：Hello World
来源：http://blog.fehbvm.com/Article/details/glskvtfpu.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/gfevgjrom.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.hesvh.cn/Article/details/gsezifpll.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fehbvm.com/Article/details/gnzdchzkm.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fehbvm.com/Article/details/gjhgagqjd.sHtML

[S03] C：读入整数
来源：http://m.share.fehbvm.com/Article/details/gwwegoaqn.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/gpcjcxuxz.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/gazsjayuw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/guxabczyn.sHtML

[S05] C：字符串长度
来源：http://baike.fehbvm.com/Article/details/gimarywgc.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/gscuxjssk.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/gbrhnglsh.sHtML

strcmp(a, b) == 0
来源：http://read.share.zdbjq.cn/Article/details/gdaoplwgi.sHtML

[S07] C：数组遍历求和
来源：http://baike.hesvh.cn/Article/details/glkptnfnz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.hesvh.cn/Article/details/gjafcwmkt.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.zdbjq.cn/Article/details/gutfwiupd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/gdcithyno.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fehbvm.com/Article/details/gkuieafjy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fehbvm.com/Article/details/gduoufqlu.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/gyuqlnwej.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/glukfdtcd.sHtML

[S11] C：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gpjijjdtq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.hesvh.cn/Article/details/gnvwkgjiz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gzgiwpfdb.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/gtnubphiy.sHtML

[S12] C：写文件
来源：http://blog.zdbjq.cn/Article/details/gfsgubexh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gtyzphhfi.sHtML

[S13] C：宏定义
来源：http://www.share.fehbvm.com/Article/details/gvzcsrzon.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/ghphbbakm.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/gvatxbjxe.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.hesvh.cn/Article/details/ghqhhxlwc.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/gisrgydgd.sHtML

(double) a / b
来源：http://m.share.fehbvm.com/Article/details/ggxzwivdt.sHtML

[S16] C：位操作置位
来源：http://wap.hesvh.cn/Article/details/gvummjdjo.sHtML

x |= (1 << 3);
来源：http://read.share.zdbjq.cn/Article/details/grtmkfcwp.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/gscwyreaa.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.zdbjq.cn/Article/details/gxhenpczx.sHtML

[S18] C：命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gsyxldmcu.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gebxunmdm.sHtML

[S19] C：快速排序
来源：http://baike.zdbjq.cn/Article/details/grfobqpoz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gglgquodt.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/ghowkcxbr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gndepvcta.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/glmdidntp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/gpweaeyiw.sHtML

[S22] C：字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/gmxlcjalt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fehbvm.com/Article/details/grdzejkkb.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/gzbtiudus.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fehbvm.com/Article/details/grnbmmdsx.sHtML

[S24] C：获取本地时间
来源：http://mobile.zdbjq.cn/Article/details/gxmbinvsj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.zdbjq.cn/Article/details/gqhlpprrz.sHtML

[S25] C：内存拷贝
来源：http://baike.hesvh.cn/Article/details/gmjzxeual.sHtML

memcpy(dst, src, n);
来源：http://3g.zdbjq.cn/Article/details/goxwbgtwq.sHtML

[S26] C：内存清零
来源：http://www.share.fehbvm.com/Article/details/gikezloht.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/gplpvxgnd.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/ghjsdkxhz.sHtML

const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gijqreqwp.sHtML

[S28] C：静态变量
来源：http://www.m.share.hesvh.cn/Article/details/gviaplatv.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/graqrqqlk.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/gyyczfscs.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fehbvm.com/Article/details/gezshywnh.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/gvgnsgvmk.sHtML

#ifndef X_H
来源：http://read.share.zdbjq.cn/Article/details/gwearpimy.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/gmkqvbajc.sHtML

#endif
来源：http://www.m.share.fehbvm.com/Article/details/gbyugoify.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gwhwmdejy.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/gadlykfkt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/ghywhsczi.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gmdgjpmuv.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/glgojznfr.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/gbjaguzos.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/guuoalkws.sHtML

[S34] C++：遍历 vector
来源：http://www.share.hesvh.cn/Article/details/gerquoozi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/gubhyunvb.sHtML

[S35] C++：map
来源：http://3g.fehbvm.com/Article/details/gssdxrdzr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gyqripzmn.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gwnblpnrd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gbjjnkudx.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/gnzlvbyjs.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.hesvh.cn/Article/details/gmutgkreh.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/ggwhqlavf.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.hesvh.cn/Article/details/goqabxzyg.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fehbvm.com/Article/details/gforcxiyi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/gcaibajyp.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/gltydenvg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.hesvh.cn/Article/details/garcmoiwx.sHtML

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/gopfxxkpe.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/giykjghei.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fehbvm.com/Article/details/gugjjmoau.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.hesvh.cn/Article/details/gsxmosxrk.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/graekxkws.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/gtizxeggf.sHtML

[S44] C++：引用传参
来源：http://www.share.fehbvm.com/Article/details/gggjevlvt.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.hesvh.cn/Article/details/guofftbvq.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/gkahpvppl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/gnobagdsh.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gwcvvwsid.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fehbvm.com/Article/details/gdpsluntw.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.zdbjq.cn/Article/details/gfxfjbhuw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/gvnanjwmg.sHtML

[S48] C++：逐行读文件
来源：http://wap.fehbvm.com/Article/details/grkbcfeod.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/gtpfllcdv.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gchiflvno.sHtML

[S49] C++：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gtrnikiom.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.zdbjq.cn/Article/details/gxtgtdyia.sHtML

[S50] C++：格式化数字
来源：http://www.share.fehbvm.com/Article/details/gzpbqdzts.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gfaohjuww.sHtML

[S51] C++：显式类型转换
来源：http://wap.hesvh.cn/Article/details/gxmlczsap.sHtML

static_cast<double>(a) / b
来源：http://mobile.zdbjq.cn/Article/details/gzvjyqkwo.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/gfaarcaij.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/gydelytjb.sHtML

[S53] C++：移动语义
来源：http://read.share.fehbvm.com/Article/details/gbsxrumwy.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/gnojtbefy.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/gwvoepsry.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.hesvh.cn/Article/details/gaasjegha.sHtML

[S55] C++：结构化绑定
来源：http://wap.zdbjq.cn/Article/details/gunliswrs.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.zdbjq.cn/Article/details/gkdeiiplt.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/gzxjdnjpe.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/gdgyapduo.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/gbehtaktd.sHtML

constexpr int N = 10;
来源：http://wap.zdbjq.cn/Article/details/gqohfftni.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/geqohmvkp.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.zdbjq.cn/Article/details/glbqpwivs.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/gcjwvgsyz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fehbvm.com/Article/details/gthwgugfx.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/gseceueji.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gyjxdtpny.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfvfvfstf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/gyrzplvrc.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grkmbfnrt.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gcgzxrhqp.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/ghwntwrbb.sHtML

[T02] Kotlin：变量
来源：http://read.share.hesvh.cn/Article/details/gppmwecfq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/gndjakpyb.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.hesvh.cn/Article/details/gcgwwwwut.sHtML

"值: $b"
来源：http://wap.hesvh.cn/Article/details/gawqkztdr.sHtML

[T04] Kotlin：空安全
来源：http://www.share.zdbjq.cn/Article/details/gptwqggyb.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/gynhjbuxe.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.zdbjq.cn/Article/details/gyokeqonf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fehbvm.com/Article/details/gdaexmbdm.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/ghjmoirwc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/goabikftj.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gloepxvke.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fehbvm.com/Article/details/gadqgpeff.sHtML

[T08] Kotlin：数据类
来源：http://blog.fehbvm.com/Article/details/gnygsiycs.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/gmnyumzbn.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/gnpeqvsau.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fehbvm.com/Article/details/gmilzgmzo.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/gmvbhkalw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.hesvh.cn/Article/details/gfhupgpkx.sHtML

[T11] Kotlin：协程
来源：http://www.share.zdbjq.cn/Article/details/gshuwydil.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.hesvh.cn/Article/details/gucogfuxi.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.hesvh.cn/Article/details/gnaeuoaqj.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gjdnpztpr.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fehbvm.com/Article/details/gbryxdpqk.sHtML

val m = mapOf("a" to 1)
来源：http://wap.zdbjq.cn/Article/details/gkrnsacoz.sHtML

[T14] Kotlin：循环
来源：http://3g.hesvh.cn/Article/details/gpdunpakv.sHtML

for (i in 1..10) println(i)
来源：http://3g.fehbvm.com/Article/details/gqrjksjni.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/gvuxfmpmo.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.hesvh.cn/Article/details/gnqtmhigh.sHtML

[T16] Swift：Hello World
来源：http://wap.fehbvm.com/Article/details/gmycvyuje.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gcwqvgpil.sHtML

[T17] Swift：变量与常量
来源：http://www.share.zdbjq.cn/Article/details/grcfqpvaz.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gsmmwnool.sHtML

[T18] Swift：字符串插值
来源：http://www.share.hesvh.cn/Article/details/grylsqahq.sHtML

"值: \(b)"
来源：http://m.share.hesvh.cn/Article/details/gxirbdofz.sHtML

[T19] Swift：可选绑定
来源：http://baike.zdbjq.cn/Article/details/glhzsqgwn.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/ggkctykgx.sHtML

[T20] Swift：数组操作
来源：http://wap.zdbjq.cn/Article/details/gadmdkkqe.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.hesvh.cn/Article/details/geqiavmuk.sHtML

[T21] Swift：遍历
来源：http://wap.fehbvm.com/Article/details/gflmzhtww.sHtML

for x in a { print(x) }
来源：http://m.share.zdbjq.cn/Article/details/gteddmida.sHtML

[T22] Swift：字典
来源：http://wap.zdbjq.cn/Article/details/gvkkbbugz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.hesvh.cn/Article/details/gdfewjwhc.sHtML

[T23] Swift：函数
来源：http://mobile.fehbvm.com/Article/details/gxyfdxilz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/gkushooth.sHtML

[T24] Swift：闭包
来源：http://mobile.zdbjq.cn/Article/details/gddvsryqh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gmawvqrhc.sHtML

[T25] Swift：结构体
来源：http://wap.fehbvm.com/Article/details/gfmtmdrzz.sHtML

struct P { var x: Int }
来源：http://read.share.zdbjq.cn/Article/details/gmawccyqh.sHtML

[T26] Swift：类与重写
来源：http://blog.fehbvm.com/Article/details/gfpciqeqq.sHtML

class A: Base { override func f() {} }
来源：http://www.share.zdbjq.cn/Article/details/gypkgsyvp.sHtML

[T27] Swift：错误处理
来源：http://m.share.fehbvm.com/Article/details/gavdezzcq.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.zdbjq.cn/Article/details/gwsfcczpt.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gegaximae.sHtML

enum Color { case red, green }
来源：http://blog.hesvh.cn/Article/details/gvkdbhdqz.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fehbvm.com/Article/details/ghzgsoxiy.sHtML

guard let x = opt else { return }
来源：http://blog.fehbvm.com/Article/details/gendnxpyf.sHtML

[T30] Swift：协议
来源：http://www.blog.hesvh.cn/Article/details/gezdcurzg.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.zdbjq.cn/Article/details/gubudvbqd.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/grhadqljo.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gdwrtqhdz.sHtML

[T32] Lua：局部变量
来源：http://wap.fehbvm.com/Article/details/gdbnhgxvq.sHtML

local a = 1
来源：http://3g.zdbjq.cn/Article/details/gmwjblykl.sHtML

[T33] Lua：表（数组）
来源：http://3g.zdbjq.cn/Article/details/gfbgbkzuj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fehbvm.com/Article/details/gxumnhtyg.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fehbvm.com/Article/details/gktedqlyo.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fehbvm.com/Article/details/gvzhlbsti.sHtML

[T35] Lua：字典表
来源：http://blog.hesvh.cn/Article/details/gzicojikt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fehbvm.com/Article/details/gnerfydlt.sHtML

[T36] Lua：函数
来源：http://www.blog.fehbvm.com/Article/details/guvwkwalu.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/gudujulvb.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gharqfpmu.sHtML

"a" .. "b"
来源：http://www.share.zdbjq.cn/Article/details/ggunyqcjn.sHtML

[T38] Lua：条件
来源：http://mobile.hesvh.cn/Article/details/guzujaoul.sHtML

if x > 0 then print("正") end
来源：http://3g.fehbvm.com/Article/details/gokkpqowh.sHtML

[T39] Lua：模式匹配
来源：http://wap.fehbvm.com/Article/details/gcjicqgug.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fehbvm.com/Article/details/ghohixoel.sHtML

[T40] Lua：元表
来源：http://www.blog.zdbjq.cn/Article/details/glwuxgwdv.sHtML

setmetatable({}, { __index = base })
来源：http://3g.hesvh.cn/Article/details/gpjssggtu.sHtML

[T41] Perl：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gvyuuheaa.sHtML

print "Hello\n";
来源：http://mobile.hesvh.cn/Article/details/glsiqkszq.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/gkkfcjsvv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fehbvm.com/Article/details/gqctloesv.sHtML


<!-- 参考信息 -->