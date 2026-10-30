代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/gldmyliek.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.hesvh.cn/Article/details/gbgyfdgsq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.zdbjq.cn/Article/details/gpjulcpip.sHtML

[R37] 把输出赋给变量
来源：http://mobile.hesvh.cn/Article/details/gzvnicqfz.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/gxuwofkhx.sHtML

[R38] 管道串联
来源：http://read.share.fehbvm.com/Article/details/gbtcvjhpy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/ggkhdfgeg.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.hesvh.cn/Article/details/gbiqylqkj.sHtML

cmd > out.log 2>&1
来源：http://blog.hesvh.cn/Article/details/ggbjxwemv.sHtML

[R40] 追加写日志
来源：http://read.share.fehbvm.com/Article/details/gnewonttp.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/gzpxuqhqm.sHtML

[R41] 丢弃输出
来源：http://mobile.zdbjq.cn/Article/details/gpoganumy.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/gxiunqraa.sHtML

[R42] 输入重定向
来源：http://wap.fehbvm.com/Article/details/grhenbgsq.sHtML

wc -l < a.txt
来源：http://read.share.fehbvm.com/Article/details/gsxojwndi.sHtML

[R43] 按名字查找文件
来源：http://mobile.hesvh.cn/Article/details/gamvkmchw.sHtML

find . -name "*.log" -type f
来源：http://www.share.zdbjq.cn/Article/details/grnsqegjx.sHtML

[R44] 按修改时间查找
来源：http://m.share.hesvh.cn/Article/details/ggdpatbrr.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gbbnuiufb.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/gihycptkh.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/gnbliwoej.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/gwesgcvze.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gwfltysfb.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/gaekpvfsj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/gxmwengnp.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/gnbmjttss.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.hesvh.cn/Article/details/guzxprhtk.sHtML

[R49] awk 带条件
来源：http://wap.hesvh.cn/Article/details/gxarpkbdl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/ggcszjiqh.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/gzttkiqmd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gryllxjhj.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/gsssxdbyc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gvodpsdtq.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/gfxltgdij.sHtML

wc -l a.txt
来源：http://read.share.fehbvm.com/Article/details/gbhshlqen.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fehbvm.com/Article/details/gkjmydewm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.hesvh.cn/Article/details/glqtdgkqd.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/gcuqauyqh.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/goulgupsf.sHtML

[R55] 压缩与解压
来源：http://m.share.hesvh.cn/Article/details/ggnqiixxi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.hesvh.cn/Article/details/gbmbtiqnm.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gmqrqdmzo.sHtML

scp file user@host:/path/
来源：http://wap.fehbvm.com/Article/details/gmiwvlnrw.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gukeethaf.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gscglktoj.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/gdakpojyt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.hesvh.cn/Article/details/gyxsracud.sHtML

[R59] 发 POST JSON
来源：http://wap.zdbjq.cn/Article/details/grrsgjpuu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/gfgbhkbbi.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/giscpfpry.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.zdbjq.cn/Article/details/gfpijitac.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/gnmrhnepw.sHtML

df -h;  du -sh *
来源：http://www.blog.hesvh.cn/Article/details/gkwezsmlc.sHtML

[R62] 找最占空间的文件
来源：http://mobile.zdbjq.cn/Article/details/gmarnzdtc.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.hesvh.cn/Article/details/gucajpmci.sHtML

[R63] 内存与进程
来源：http://www.share.hesvh.cn/Article/details/gdzfhwmlk.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.zdbjq.cn/Article/details/ggjoypcqj.sHtML

[R64] 结束进程
来源：http://wap.zdbjq.cn/Article/details/ggxemjohh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/gysoxygsk.sHtML

[R65] 查看端口占用
来源：http://wap.hesvh.cn/Article/details/gvcjhlgie.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/gosdhaakd.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gaglamphi.sHtML

crontab -e;  crontab -l
来源：http://m.share.fehbvm.com/Article/details/gqpegcyov.sHtML

[R67] 生成随机十六进制串
来源：http://wap.zdbjq.cn/Article/details/gsgqqtysu.sHtML

openssl rand -hex 16
来源：http://m.share.hesvh.cn/Article/details/ggrxklrdo.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/goukmroat.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.hesvh.cn/Article/details/gtjkbyhah.sHtML

[R69] 生成随机密码
来源：http://www.blog.hesvh.cn/Article/details/gitvunxqi.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gppebqbcc.sHtML

[R70] 时间戳与互转
来源：http://3g.zdbjq.cn/Article/details/grpygrirs.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gskkxszoj.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gdpwkdxzw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/gqjkhspjv.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gecknjrqh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gdgznrpqm.sHtML

[R73] 分割大日志
来源：http://www.m.share.fehbvm.com/Article/details/gxeyowbkp.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/gikgoinwt.sHtML

[R74] 批量重命名
来源：http://wap.fehbvm.com/Article/details/gkooxljwa.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.zdbjq.cn/Article/details/gwfvudpfl.sHtML

[R75] 导出环境变量
来源：http://3g.hesvh.cn/Article/details/gwucrnkhl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.zdbjq.cn/Article/details/gebfdwkzk.sHtML

[R76] 使用临时文件
来源：http://www.blog.fehbvm.com/Article/details/gctezxhcb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gfnqwdmsi.sHtML

[R77] 读取用户输入
来源：http://wap.hesvh.cn/Article/details/gandhwcnu.sHtML

read -rp "请输入: " ans
来源：http://3g.zdbjq.cn/Article/details/gaxrhxviy.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/gssnzrhjh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/gmzbkcnnt.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/gyjvvigsh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/gtzcayvrc.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.hesvh.cn/Article/details/gnsnysmsr.sHtML

time ./run.sh
来源：http://www.blog.fehbvm.com/Article/details/gwyfnmbnj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grjvugahe.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gndxrmszt.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gghtaefmo.sHtML

[S01] C：Hello World
来源：http://baike.zdbjq.cn/Article/details/gimdxikxy.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/gocudzbcb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gxexvkslx.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/gtczwklhd.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.hesvh.cn/Article/details/gzpselzgq.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/gsliflccz.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/gpspzieed.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/gazpitvsd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/gcacwwzsl.sHtML

[S05] C：字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gyeufppuu.sHtML

strlen(s)
来源：http://read.share.zdbjq.cn/Article/details/gysnmczkr.sHtML

[S06] C：字符串比较
来源：http://www.share.fehbvm.com/Article/details/ghfmlqrlc.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/gheqdtbcb.sHtML

[S07] C：数组遍历求和
来源：http://baike.hesvh.cn/Article/details/gzxgbnsjl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.hesvh.cn/Article/details/ghjhznzmb.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.hesvh.cn/Article/details/gmgrkiiub.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fehbvm.com/Article/details/gulboweyh.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.hesvh.cn/Article/details/gsqgcptru.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/goxenzajf.sHtML

[S10] C：指针与解引用
来源：http://www.share.fehbvm.com/Article/details/gsoimrybj.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/gvguktizf.sHtML

[S11] C：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gdsweauuc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.hesvh.cn/Article/details/ghobskldy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.hesvh.cn/Article/details/ghjjxmeni.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/ggborqoto.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/ganhwimai.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gkpulehez.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/gfxfqiybu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/gfzgvdsji.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/gjqengsxl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/gdreqglvn.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/guxldwasa.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/gmwbwwqtl.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gzubkolbt.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/goeheuyey.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/grchtqzic.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/ghxjblepl.sHtML

[S18] C：命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gcmmpiaru.sHtML

int main(int argc, char **argv)
来源：http://mobile.hesvh.cn/Article/details/gimdzxmha.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/giivfoxqo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gkinulbap.sHtML

[S20] C：二分查找
来源：http://mobile.hesvh.cn/Article/details/gryasdjsi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gmebtoecr.sHtML

[S21] C：字符类别判断
来源：http://www.share.fehbvm.com/Article/details/gigrfpzld.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fehbvm.com/Article/details/gcjxkinxl.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/gsjjjwtkb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.hesvh.cn/Article/details/gybljpgpu.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/gaggaxicn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/gwmegvgib.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/gtwrdiacq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/gompfuksd.sHtML

[S25] C：内存拷贝
来源：http://read.share.zdbjq.cn/Article/details/gprtxtyou.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gdllhzkay.sHtML

[S26] C：内存清零
来源：http://m.share.fehbvm.com/Article/details/gtxafkpgn.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fehbvm.com/Article/details/gwnxpuqie.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/ggfsbysui.sHtML

const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gdisuwhrr.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/gyadajmtt.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gevzekndd.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/gmsiegskb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fehbvm.com/Article/details/gdooqudmf.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/gnsxndync.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/grogtcriz.sHtML

#define X_H
来源：http://mobile.hesvh.cn/Article/details/grhxacicm.sHtML

#endif
来源：http://www.m.share.zdbjq.cn/Article/details/gomcwclnq.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/guabhxtrv.sHtML

#include <iostream>
来源：http://baike.hesvh.cn/Article/details/gswqiofur.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.hesvh.cn/Article/details/gpiwdqkpr.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/gqzewdkkc.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/gakjfkstz.sHtML

[S33] C++：vector 增删
来源：http://mobile.zdbjq.cn/Article/details/gnvgcwwia.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/ghrujlspp.sHtML

[S34] C++：遍历 vector
来源：http://baike.hesvh.cn/Article/details/gayggdqeg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/gcwjhlutr.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/gffzpnlei.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gsumiceid.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fehbvm.com/Article/details/gnbqyjmwo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/guqsrvulp.sHtML

[S37] C++：set
来源：http://www.share.zdbjq.cn/Article/details/gufkspzoj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fehbvm.com/Article/details/gfclceurh.sHtML

[S38] C++：排序
来源：http://www.share.zdbjq.cn/Article/details/gyvatjvhc.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fehbvm.com/Article/details/ghhyxwrok.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fehbvm.com/Article/details/glfkjxrht.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.hesvh.cn/Article/details/gjnsizyjk.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/gttpplevj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/geqibxkko.sHtML

[S41] C++：类与构造函数
来源：http://www.share.hesvh.cn/Article/details/gpprpigii.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.zdbjq.cn/Article/details/gnjsgcjzo.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/grmouweej.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.zdbjq.cn/Article/details/geiddtqjd.sHtML

[S43] C++：智能指针
来源：http://www.share.hesvh.cn/Article/details/ggmycwbvb.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.hesvh.cn/Article/details/gcsdttjrs.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/grhihcwqz.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.zdbjq.cn/Article/details/gunbgbpgf.sHtML

[S45] C++：lambda
来源：http://blog.fehbvm.com/Article/details/gtddlekey.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/gudvzskyb.sHtML

[S46] C++：函数模板
来源：http://wap.zdbjq.cn/Article/details/grrcumzjt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/gbkikwceo.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.hesvh.cn/Article/details/gvvkegfnt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/gcfpnrska.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gcfyjksfe.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.hesvh.cn/Article/details/gwzptcnma.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gcjormrfk.sHtML

[S49] C++：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gtthupqnk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.hesvh.cn/Article/details/gtiqmomoc.sHtML

[S50] C++：格式化数字
来源：http://blog.hesvh.cn/Article/details/ggkwagwgx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/gazinsegl.sHtML

[S51] C++：显式类型转换
来源：http://mobile.hesvh.cn/Article/details/gmirbxpsv.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fehbvm.com/Article/details/gkrsbjdwt.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/gucertvtq.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/gyojyvqdl.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/goheotbxs.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/gvcslcvsm.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fehbvm.com/Article/details/gymfexjno.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.zdbjq.cn/Article/details/glfuzscbl.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/gfowlggao.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/glbrszctx.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/gxtwnayme.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.hesvh.cn/Article/details/gtjtbjkqx.sHtML

[S57] C++：编译期常量
来源：http://blog.hesvh.cn/Article/details/gjuspzhzk.sHtML

constexpr int N = 10;
来源：http://www.m.share.hesvh.cn/Article/details/grftjictc.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/gsluotyte.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.hesvh.cn/Article/details/gvnbuqfpq.sHtML

[S59] C++：静态断言
来源：http://www.share.hesvh.cn/Article/details/gzrvosqbf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gmyuwcivs.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.hesvh.cn/Article/details/gqouydzac.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gpjxgkjdh.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpttzknup.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gjvuiroah.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gymxwjuzt.sHtML

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/gvyigkbam.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/ghrjpcwtp.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/gtagyxjrx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.hesvh.cn/Article/details/gvattjolv.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/guokrviaj.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/ghadkbihr.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/gxwoqyglc.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/gcqrtxfba.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/gtycfguzb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/ggdqqugkm.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/gxtcltxjr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/glncahqhz.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gswujqbqg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.hesvh.cn/Article/details/gabkzgyfd.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fehbvm.com/Article/details/gpdngicua.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gkvsqloeu.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.zdbjq.cn/Article/details/grseerbdl.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fehbvm.com/Article/details/gitlaetht.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fehbvm.com/Article/details/gzunzhsnd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/gmmpqtvlo.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fehbvm.com/Article/details/gvrqkfezz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.zdbjq.cn/Article/details/gbjihmjvf.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fehbvm.com/Article/details/ghnurtrgi.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gugjhgngy.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.zdbjq.cn/Article/details/gvnirsmzy.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.zdbjq.cn/Article/details/gugabrnpe.sHtML

[T14] Kotlin：循环
来源：http://m.share.hesvh.cn/Article/details/gqffpazwo.sHtML

for (i in 1..10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gvsonwrqk.sHtML

[T15] Kotlin：接口
来源：http://wap.fehbvm.com/Article/details/gxrfkgxqk.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.hesvh.cn/Article/details/gfnvymlxf.sHtML

[T16] Swift：Hello World
来源：http://wap.zdbjq.cn/Article/details/gzermawhd.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gcmriipjb.sHtML

[T17] Swift：变量与常量
来源：http://baike.fehbvm.com/Article/details/gvoohzmab.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/gagamzimd.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gbbfazpal.sHtML

"值: \(b)"
来源：http://www.blog.zdbjq.cn/Article/details/gkbkgwmpz.sHtML

[T19] Swift：可选绑定
来源：http://www.share.zdbjq.cn/Article/details/gmmkzajhd.sHtML

if let n = opt { print(n) }
来源：http://m.share.zdbjq.cn/Article/details/gtldeqqtv.sHtML

[T20] Swift：数组操作
来源：http://3g.fehbvm.com/Article/details/gvivdxymy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.zdbjq.cn/Article/details/gvwaudvtr.sHtML

[T21] Swift：遍历
来源：http://m.share.zdbjq.cn/Article/details/giexxvpym.sHtML

for x in a { print(x) }
来源：http://m.share.zdbjq.cn/Article/details/ggvdkgiel.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/gfnvbmxui.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.hesvh.cn/Article/details/gxfqjkeyv.sHtML

[T23] Swift：函数
来源：http://3g.fehbvm.com/Article/details/ggbrnanlr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.zdbjq.cn/Article/details/gqohbkeez.sHtML

[T24] Swift：闭包
来源：http://wap.zdbjq.cn/Article/details/gxculftxg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gakhuvcgr.sHtML

[T25] Swift：结构体
来源：http://www.m.share.hesvh.cn/Article/details/gspzbjlcd.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/gsazswkjx.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/gpjaxsevj.sHtML

class A: Base { override func f() {} }
来源：http://3g.hesvh.cn/Article/details/gflevticc.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/gdptohwgv.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fehbvm.com/Article/details/gjyrmbcyq.sHtML

[T28] Swift：枚举
来源：http://baike.zdbjq.cn/Article/details/glyvnqlaq.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/grfcwhsuz.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fehbvm.com/Article/details/gpbygfjer.sHtML

guard let x = opt else { return }
来源：http://mobile.hesvh.cn/Article/details/gencfgigv.sHtML

[T30] Swift：协议
来源：http://wap.hesvh.cn/Article/details/gprlqoixb.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.hesvh.cn/Article/details/gsutitdtt.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gxnhfhwox.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gdafuovag.sHtML

[T32] Lua：局部变量
来源：http://mobile.hesvh.cn/Article/details/gfwkjesfc.sHtML

local a = 1
来源：http://blog.zdbjq.cn/Article/details/gglmqvtkt.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.hesvh.cn/Article/details/gdikuocmb.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.hesvh.cn/Article/details/gzzoecfps.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/gzlybuwol.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.hesvh.cn/Article/details/gcewsbncd.sHtML

[T35] Lua：字典表
来源：http://wap.hesvh.cn/Article/details/gpihdnmom.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.hesvh.cn/Article/details/gbhjfikog.sHtML

[T36] Lua：函数
来源：http://m.share.hesvh.cn/Article/details/gvaasebva.sHtML

function add(a, b) return a + b end
来源：http://blog.hesvh.cn/Article/details/gulminpjl.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fehbvm.com/Article/details/ghtdcxlnb.sHtML

"a" .. "b"
来源：http://3g.zdbjq.cn/Article/details/gsgdufeng.sHtML

[T38] Lua：条件
来源：http://wap.hesvh.cn/Article/details/ggnvyewkm.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/gxejdefqb.sHtML


<!-- 参考信息 -->