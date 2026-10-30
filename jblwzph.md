代发 wailian999

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/gagjgysfu.sHtML

[R40] 追加写日志
来源：http://www.share.zdbjq.cn/Article/details/gcurjdctl.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/gpllyzjor.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/gbepyxuzq.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gtqycgovs.sHtML

[R42] 输入重定向
来源：http://www.share.fehbvm.com/Article/details/gjzcvozte.sHtML

wc -l < a.txt
来源：http://www.blog.zdbjq.cn/Article/details/geunhaadk.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/gswszdsdp.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/gskayowuk.sHtML

[R44] 按修改时间查找
来源：http://wap.zdbjq.cn/Article/details/gyyhvhpxs.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/geulotknv.sHtML

[R45] 批量删除
来源：http://m.share.hesvh.cn/Article/details/gpghipdvg.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/gqpjdpcsh.sHtML

[R46] 递归替换文件内容
来源：http://m.share.zdbjq.cn/Article/details/ghmogiwvt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.hesvh.cn/Article/details/gnzmtexbr.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/ghuddhnjo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.hesvh.cn/Article/details/gkeqgjrfl.sHtML

[R48] awk 取指定列
来源：http://www.blog.hesvh.cn/Article/details/gkmqwkmui.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gkjcxhabw.sHtML

[R49] awk 带条件
来源：http://blog.hesvh.cn/Article/details/gntuhusmc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.hesvh.cn/Article/details/gxihltynd.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/gstacgnkb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/gtclbkwjh.sHtML

[R51] 排序去重取前几
来源：http://www.blog.hesvh.cn/Article/details/gfiluflda.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/goinkrmyp.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/gcvxuywle.sHtML

wc -l a.txt
来源：http://www.blog.fehbvm.com/Article/details/gonbtsydi.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.zdbjq.cn/Article/details/gdyilrncp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/gksboesgs.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/gesxphozi.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/gqvjkedkn.sHtML

[R55] 压缩与解压
来源：http://read.share.hesvh.cn/Article/details/gtzupsihe.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.hesvh.cn/Article/details/geokfsqxg.sHtML

[R56] 远程拷贝
来源：http://baike.hesvh.cn/Article/details/gadjvogon.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/gqxyyonta.sHtML

[R57] 远程执行命令
来源：http://m.share.hesvh.cn/Article/details/gckxfpqdv.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/ghpudjhpt.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/gusurmhad.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.zdbjq.cn/Article/details/gipgrtrvf.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gbadovkfx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fehbvm.com/Article/details/gmlczdxgc.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gawjlxapd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.zdbjq.cn/Article/details/gdojrpuif.sHtML

[R61] 磁盘占用
来源：http://baike.fehbvm.com/Article/details/gzichfbxv.sHtML

df -h;  du -sh *
来源：http://baike.zdbjq.cn/Article/details/gausmcfob.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.hesvh.cn/Article/details/gvajnzqel.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.hesvh.cn/Article/details/gxsletsnr.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/guvmvypfc.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/gyzyehigt.sHtML

[R64] 结束进程
来源：http://www.share.fehbvm.com/Article/details/glznzwilx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fehbvm.com/Article/details/gkptljpuz.sHtML

[R65] 查看端口占用
来源：http://www.blog.hesvh.cn/Article/details/gmnjkskfm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.zdbjq.cn/Article/details/gjejygmdt.sHtML

[R66] 定时任务
来源：http://baike.zdbjq.cn/Article/details/gmcncmjon.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/gedoblzgm.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/gtumtqowu.sHtML

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/goiyzhtci.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/gwlqwfkna.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.zdbjq.cn/Article/details/guuhburbo.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/gjigtloql.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/gbmctywnm.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/gjpzvzumm.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gybvxfbqr.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gyfpwvycl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/gkknjkvqn.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gxsuqezoj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gmnxeirbk.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gsdntlioa.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/ghtsezcbd.sHtML

[R74] 批量重命名
来源：http://m.share.fehbvm.com/Article/details/gydmjbpfg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/gcwamrxcp.sHtML

[R75] 导出环境变量
来源：http://read.share.fehbvm.com/Article/details/gksdgqeud.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.zdbjq.cn/Article/details/gzgvgxenm.sHtML

[R76] 使用临时文件
来源：http://www.blog.hesvh.cn/Article/details/gawbaotoq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gbufddwhp.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/gfctbooms.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/gocamuxsh.sHtML

[R78] 交互式菜单
来源：http://www.blog.fehbvm.com/Article/details/gkwffgqxe.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.hesvh.cn/Article/details/gkanjrnhe.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/gmhujtsyk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/gazgenvya.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/gqkycielk.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/gesqpxzdx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqragqukm.sHtML

S. C / C++ 专题
来源：http://wap.hesvh.cn/Article/details/gnjjcbhbw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmhtuvosu.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gjgemnnab.sHtML

#include <stdio.h>
来源：http://wap.hesvh.cn/Article/details/gbxfdeasc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gvvhreors.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/gopurvqdc.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/gouaztxyv.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/gvsnznpfp.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/gyzhsvuab.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/gaqsawfyd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.hesvh.cn/Article/details/gyfcvbggw.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/ginvipixi.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/gusgbtldv.sHtML

[S06] C：字符串比较
来源：http://baike.hesvh.cn/Article/details/gdtlyvnhd.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/gkvxtnqzg.sHtML

[S07] C：数组遍历求和
来源：http://baike.zdbjq.cn/Article/details/glvzxgzla.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gtjevrlgx.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.hesvh.cn/Article/details/gmemvkmad.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/glpvpolfu.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.hesvh.cn/Article/details/gvqfdthdd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/golpnwqcz.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/gidwhmzcp.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fehbvm.com/Article/details/giesyjydv.sHtML

[S11] C：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gyypxwoja.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gpjthbwab.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.zdbjq.cn/Article/details/gywfxeils.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gytzljlzx.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/gwbazbgmm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gvzionwvb.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/gvdjrfmpk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fehbvm.com/Article/details/gfffpcoty.sHtML

[S14] C：枚举
来源：http://3g.hesvh.cn/Article/details/gsxwdxwnz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/gxbbbikwd.sHtML

[S15] C：类型转换
来源：http://m.share.fehbvm.com/Article/details/gzsaitcih.sHtML

(double) a / b
来源：http://3g.hesvh.cn/Article/details/gfhotphoz.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/gthqtfyvk.sHtML

x |= (1 << 3);
来源：http://www.share.zdbjq.cn/Article/details/gothqmtmp.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gmkvbfefp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gblooqqez.sHtML

[S18] C：命令行参数
来源：http://3g.fehbvm.com/Article/details/gnarldmwi.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/gipjexpki.sHtML

[S19] C：快速排序
来源：http://blog.hesvh.cn/Article/details/giqculhef.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gabpwmgyi.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/gpcdrkhyn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gidqromnq.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/gzedmisym.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/gzkalvahj.sHtML

[S22] C：字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gxvjihjpa.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/gznmmdopm.sHtML

[S23] C：随机数
来源：http://mobile.hesvh.cn/Article/details/gullsehjy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/gomlyyzqd.sHtML

[S24] C：获取本地时间
来源：http://3g.hesvh.cn/Article/details/ghtwrjpya.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.zdbjq.cn/Article/details/gntceiizp.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/glusgjfbi.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fehbvm.com/Article/details/gmhhjgepy.sHtML

[S26] C：内存清零
来源：http://baike.fehbvm.com/Article/details/gvzggvwmu.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/ghyzhjtky.sHtML

[S27] C：定义常量
来源：http://mobile.fehbvm.com/Article/details/gpnnzrhax.sHtML

const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/glxlbpdji.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/gfjvuzodo.sHtML

static int counter = 0;
来源：http://m.share.fehbvm.com/Article/details/gxantqxft.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/gepmgiqpr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.hesvh.cn/Article/details/gzrllojea.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gwpwhqhrc.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/gsqwhfywg.sHtML

#define X_H
来源：http://3g.zdbjq.cn/Article/details/giuayffon.sHtML

#endif
来源：http://www.blog.fehbvm.com/Article/details/gtktzbeyq.sHtML

[S31] C++：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gcqbvplno.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/gwojorfvf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/ghymiourk.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/gngzytzdp.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/gwlxecxmg.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.zdbjq.cn/Article/details/gecylcedx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/givfoouoj.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/gablmolkd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/gtbvibrfq.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/ghnnedink.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gwahgrvvk.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/gddfarwzp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gpvdynepi.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/gpkjmlcma.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fehbvm.com/Article/details/gvgljotrv.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/gniydcjnl.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gatflwcqv.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/gnhuvxgfo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fehbvm.com/Article/details/gdolgenes.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/gxspdgeyq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/gkjwmlpdf.sHtML

[S41] C++：类与构造函数
来源：http://read.share.hesvh.cn/Article/details/gjclemvqs.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.zdbjq.cn/Article/details/gfwfdlpkz.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/gxgsibhuw.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/gcjrjuzbp.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gunzvhvio.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/gwfgcpwiu.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/gmwkaugqj.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fehbvm.com/Article/details/gdoliwriu.sHtML

[S45] C++：lambda
来源：http://www.share.zdbjq.cn/Article/details/gqecowulk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/gtgnfkuqa.sHtML

[S46] C++：函数模板
来源：http://www.m.share.zdbjq.cn/Article/details/gyohzntid.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/gmcwstkyz.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/ghlfelnda.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.zdbjq.cn/Article/details/gdukqlhzg.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gcnmwrkwi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fehbvm.com/Article/details/ghnyktnic.sHtML

while (std::getline(in, line)) { }
来源：http://blog.hesvh.cn/Article/details/gfznxiyqi.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/gdnnymglt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.zdbjq.cn/Article/details/grgwtauga.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fehbvm.com/Article/details/gidqguqtm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/giirhnxfm.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/gjarjsqxb.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gakkztrvf.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/gymysjppu.sHtML

int size() const noexcept { return n_; }
来源：http://baike.hesvh.cn/Article/details/gqrqcytrv.sHtML

[S53] C++：移动语义
来源：http://mobile.fehbvm.com/Article/details/gwcboixhq.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.hesvh.cn/Article/details/gofvoqmyh.sHtML

[S54] C++：异常处理
来源：http://m.share.zdbjq.cn/Article/details/gtseteija.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.hesvh.cn/Article/details/gopihwkrr.sHtML

[S55] C++：结构化绑定
来源：http://read.share.zdbjq.cn/Article/details/ghauhxjat.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.hesvh.cn/Article/details/gqyvyzbqo.sHtML

[S56] C++：optional
来源：http://blog.fehbvm.com/Article/details/gbuwmvqtp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.hesvh.cn/Article/details/ggfiohtpi.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/gvbrkamoj.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/gqgwxokdo.sHtML

[S58] C++：命名空间
来源：http://read.share.fehbvm.com/Article/details/gcfkpfomo.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.zdbjq.cn/Article/details/gaewccror.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/giyqlmpos.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fehbvm.com/Article/details/ghfdejlfj.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gncqivqzv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.zdbjq.cn/Article/details/gclxfqbqs.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/giawuzird.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gojmmmhge.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmpagdnef.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fehbvm.com/Article/details/gjrwexzvh.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gmtcquijs.sHtML

[T02] Kotlin：变量
来源：http://mobile.zdbjq.cn/Article/details/guecxmvqi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/goqmeelgv.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.zdbjq.cn/Article/details/gtxihsjce.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/ghchxaaiq.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/gryeyytsj.sHtML

val n: String? = null;  n?.length
来源：http://mobile.hesvh.cn/Article/details/ghzriyvaj.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.hesvh.cn/Article/details/gkhvqhccj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fehbvm.com/Article/details/ggcevsjbb.sHtML

[T06] Kotlin：集合映射
来源：http://3g.zdbjq.cn/Article/details/gxdlxkizp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.hesvh.cn/Article/details/gojyltzry.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gkyxeqvfe.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/gavteveii.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fehbvm.com/Article/details/guibgmqsn.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.hesvh.cn/Article/details/gznrrtirc.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.zdbjq.cn/Article/details/gjwcvnubl.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fehbvm.com/Article/details/gcernuogv.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fehbvm.com/Article/details/guiuewcqp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/gbtlreorw.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/grgmocphy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/gpanlpner.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/grzxlzuge.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gtdcawxjh.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fehbvm.com/Article/details/guziuhkto.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.zdbjq.cn/Article/details/gbogxsnbo.sHtML

[T14] Kotlin：循环
来源：http://mobile.zdbjq.cn/Article/details/gpddvqolx.sHtML

for (i in 1..10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gpzapwctz.sHtML

[T15] Kotlin：接口
来源：http://m.share.fehbvm.com/Article/details/gwcrtebeb.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/guvvpdqtp.sHtML

[T16] Swift：Hello World
来源：http://blog.zdbjq.cn/Article/details/gqgqkzfzl.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gcpmfnewt.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/gwwtyqpua.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/gfdumtkmh.sHtML

[T18] Swift：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gtyostzrd.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/gmltlvizj.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gdsnmfqbu.sHtML

if let n = opt { print(n) }
来源：http://wap.hesvh.cn/Article/details/gybrsnuyg.sHtML

[T20] Swift：数组操作
来源：http://m.share.fehbvm.com/Article/details/gayswtqrr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/ggreuxwyj.sHtML

[T21] Swift：遍历
来源：http://blog.zdbjq.cn/Article/details/gcqjtibqw.sHtML

for x in a { print(x) }
来源：http://www.blog.fehbvm.com/Article/details/gsefqrndn.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/gwtlbmpkk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.hesvh.cn/Article/details/guqfxejtv.sHtML

[T23] Swift：函数
来源：http://wap.zdbjq.cn/Article/details/gbqeviijw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fehbvm.com/Article/details/gipcnrlbx.sHtML

[T24] Swift：闭包
来源：http://www.blog.hesvh.cn/Article/details/ghmyunsjt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fehbvm.com/Article/details/gfsgwnphv.sHtML

[T25] Swift：结构体
来源：http://m.share.hesvh.cn/Article/details/gtdagejlw.sHtML

struct P { var x: Int }
来源：http://baike.zdbjq.cn/Article/details/ghqezbikr.sHtML

[T26] Swift：类与重写
来源：http://read.share.hesvh.cn/Article/details/gzhuivccv.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gpqdslaoa.sHtML

[T27] Swift：错误处理
来源：http://wap.fehbvm.com/Article/details/gkiotjssi.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fehbvm.com/Article/details/gkxthxvxl.sHtML

[T28] Swift：枚举
来源：http://read.share.hesvh.cn/Article/details/gvykfiurg.sHtML

enum Color { case red, green }
来源：http://www.m.share.zdbjq.cn/Article/details/gpgrthyjz.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fehbvm.com/Article/details/gagilvpme.sHtML

guard let x = opt else { return }
来源：http://baike.fehbvm.com/Article/details/gebdlcmlc.sHtML

[T30] Swift：协议
来源：http://read.share.zdbjq.cn/Article/details/gxzjyfulj.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.hesvh.cn/Article/details/ggqciaaur.sHtML

[T31] Lua：Hello World
来源：http://www.share.fehbvm.com/Article/details/glwsqszeo.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/geailcadk.sHtML

[T32] Lua：局部变量
来源：http://www.share.zdbjq.cn/Article/details/grcalarjt.sHtML

local a = 1
来源：http://www.blog.zdbjq.cn/Article/details/gzmgqjjbq.sHtML

[T33] Lua：表（数组）
来源：http://mobile.zdbjq.cn/Article/details/gnbqjtvwt.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fehbvm.com/Article/details/gwmxdlimq.sHtML

[T34] Lua：遍历表
来源：http://baike.fehbvm.com/Article/details/gqitzqxym.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.zdbjq.cn/Article/details/gxeuzxtae.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/gylbqgztl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gmdioutgv.sHtML

[T36] Lua：函数
来源：http://www.m.share.fehbvm.com/Article/details/ghnsldzfk.sHtML

function add(a, b) return a + b end
来源：http://wap.fehbvm.com/Article/details/gnvovmysk.sHtML

[T37] Lua：字符串拼接
来源：http://blog.hesvh.cn/Article/details/gzhcthsbq.sHtML

"a" .. "b"
来源：http://wap.zdbjq.cn/Article/details/gzrqhvdih.sHtML

[T38] Lua：条件
来源：http://mobile.fehbvm.com/Article/details/gmauprrcs.sHtML

if x > 0 then print("正") end
来源：http://blog.zdbjq.cn/Article/details/gvsyabuog.sHtML

[T39] Lua：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gewaiutra.sHtML

string.find(s, "%d+")
来源：http://baike.hesvh.cn/Article/details/gygrvxdel.sHtML

[T40] Lua：元表
来源：http://read.share.hesvh.cn/Article/details/gvwtwotjh.sHtML

setmetatable({}, { __index = base })
来源：http://wap.hesvh.cn/Article/details/gdancpatp.sHtML

[T41] Perl：Hello World
来源：http://blog.zdbjq.cn/Article/details/gnjhgtvsa.sHtML

print "Hello\n";
来源：http://mobile.hesvh.cn/Article/details/glmyzzwzm.sHtML

[T42] Perl：变量类型
来源：http://3g.fehbvm.com/Article/details/gtgmkageg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fehbvm.com/Article/details/gplcxvjev.sHtML


<!-- 参考信息 -->