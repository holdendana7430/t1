代发 wailian999

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/ghgvvrapo.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/glquflzhl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.zdbjq.cn/Article/details/guufmwavb.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fehbvm.com/Article/details/gdemyxcey.sHtML

cmd > out.log 2>&1
来源：http://3g.fehbvm.com/Article/details/gtijhjvfc.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/gxpoiowrg.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/gjahouovf.sHtML

[R41] 丢弃输出
来源：http://www.share.zdbjq.cn/Article/details/grqxievfu.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/gyrgdgcoe.sHtML

[R42] 输入重定向
来源：http://wap.fehbvm.com/Article/details/giucsnxtq.sHtML

wc -l < a.txt
来源：http://baike.zdbjq.cn/Article/details/grzdhmkhu.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/gihrsbnmx.sHtML

find . -name "*.log" -type f
来源：http://m.share.hesvh.cn/Article/details/gbupflwkb.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/gsrmwouyz.sHtML

find . -mtime -7 -type f
来源：http://www.blog.zdbjq.cn/Article/details/gzkpwydik.sHtML

[R45] 批量删除
来源：http://blog.zdbjq.cn/Article/details/gpoxwbmfu.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/gafxwpufw.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fehbvm.com/Article/details/gfgjszfko.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.zdbjq.cn/Article/details/gqcwwbewg.sHtML

[R47] sed 单行替换
来源：http://mobile.fehbvm.com/Article/details/gdgkwshpo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/ggzhwertn.sHtML

[R48] awk 取指定列
来源：http://read.share.fehbvm.com/Article/details/gtuxsohrr.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/glyoplcab.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/grsoxvgay.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/gpthuxmde.sHtML

[R50] awk 求和
来源：http://www.blog.zdbjq.cn/Article/details/gjidnqamo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gculmbllt.sHtML

[R51] 排序去重取前几
来源：http://www.share.fehbvm.com/Article/details/gzrnhxeji.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/gwgwkikzq.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/gblbvxqqb.sHtML

wc -l a.txt
来源：http://mobile.zdbjq.cn/Article/details/gswjgqduo.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/gknyykkgk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fehbvm.com/Article/details/ghzqbwsdv.sHtML

[R54] 比较两个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gkbrectgk.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/gmamocvaq.sHtML

[R55] 压缩与解压
来源：http://m.share.zdbjq.cn/Article/details/gijcdguuv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.hesvh.cn/Article/details/gobcrdvjn.sHtML

[R56] 远程拷贝
来源：http://baike.fehbvm.com/Article/details/guycpzrhh.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/gqoxiwnhy.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/gudcukgjy.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/gshivsykm.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/girvbogmr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.hesvh.cn/Article/details/gjznsycqw.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gbmvyeetx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fehbvm.com/Article/details/gyptbyjgj.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/guvzafprg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fehbvm.com/Article/details/gosbtnbwf.sHtML

[R61] 磁盘占用
来源：http://m.share.zdbjq.cn/Article/details/gyopmlczt.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/gxeuvqqcn.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/gjewljtwn.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fehbvm.com/Article/details/gjbcdlrpq.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gcuatbuky.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/gzjnrghqj.sHtML

[R64] 结束进程
来源：http://www.blog.hesvh.cn/Article/details/gbbpdaawo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/gdqptplje.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/gkmrksvpg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.hesvh.cn/Article/details/gpbrlsggw.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/golvcrqlc.sHtML

crontab -e;  crontab -l
来源：http://blog.fehbvm.com/Article/details/gbmstzeax.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.hesvh.cn/Article/details/gyengfqso.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/gdtuulgsi.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/gpywhdtuu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fehbvm.com/Article/details/gutbreiqo.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/gxxzbuhqy.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/gbdihfrml.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/gfvzphrre.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.hesvh.cn/Article/details/gyltpqjhu.sHtML

[R71] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gicuujrsg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/glkeqpatp.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/gkkdpxian.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gscrcpimj.sHtML

[R73] 分割大日志
来源：http://read.share.hesvh.cn/Article/details/ggbuoailt.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/gsiabpxil.sHtML

[R74] 批量重命名
来源：http://m.share.zdbjq.cn/Article/details/grlhwysfr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.zdbjq.cn/Article/details/gualqbrbl.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/ggpwuabcc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.zdbjq.cn/Article/details/grfrmmyxt.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/gzyxlcmct.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gdhdyishj.sHtML

[R77] 读取用户输入
来源：http://mobile.fehbvm.com/Article/details/gctwwjmhy.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/gypbbxxsy.sHtML

[R78] 交互式菜单
来源：http://www.m.share.hesvh.cn/Article/details/gquxwkdtc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/gpysrkopg.sHtML

[R79] 解析命令行选项
来源：http://www.share.zdbjq.cn/Article/details/gbifqiiht.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.zdbjq.cn/Article/details/ggokulzdt.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gsryzufrj.sHtML

time ./run.sh
来源：http://www.blog.fehbvm.com/Article/details/godmpcbih.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjfxvwhnp.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gisjxleht.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggvthfysn.sHtML

[S01] C：Hello World
来源：http://mobile.fehbvm.com/Article/details/gfeypolgo.sHtML

#include <stdio.h>
来源：http://blog.fehbvm.com/Article/details/gfzhzsewn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/gseerwdmw.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/gvlhshuwl.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.zdbjq.cn/Article/details/gjpkdfmhu.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/goznpznyj.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/gnuirchci.sHtML

[S04] C：字符串复制
来源：http://read.share.fehbvm.com/Article/details/ggbqoqmna.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fehbvm.com/Article/details/ghygjzuhn.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gjgsweqpb.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/gbtyqhfjf.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/gnpvuunfq.sHtML

strcmp(a, b) == 0
来源：http://www.share.zdbjq.cn/Article/details/gcotzwytc.sHtML

[S07] C：数组遍历求和
来源：http://3g.zdbjq.cn/Article/details/gvteyfpyp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.hesvh.cn/Article/details/gshqvxssc.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/gozsbhjdd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/gkuqnakjn.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.hesvh.cn/Article/details/gbxfqchro.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/ghqipbecc.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/gmpzjuckn.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/gecfruhej.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gyyushwmp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.zdbjq.cn/Article/details/gmvhpcrwv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.zdbjq.cn/Article/details/glpewwgwe.sHtML

fclose(f);
来源：http://wap.hesvh.cn/Article/details/gkwvfnmij.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/gxixtgaub.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/gucatcoct.sHtML

[S13] C：宏定义
来源：http://www.share.zdbjq.cn/Article/details/gclcynnjo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.zdbjq.cn/Article/details/gjpevnupa.sHtML

[S14] C：枚举
来源：http://www.blog.hesvh.cn/Article/details/gpxgtnbvq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/gvpubjxtc.sHtML

[S15] C：类型转换
来源：http://baike.zdbjq.cn/Article/details/gmblexsfh.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/gmoxuakbm.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/ghfkuicuq.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/gvdujctoh.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gjbvtxwsy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/gxfovgnzy.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/gswmsnjxv.sHtML

int main(int argc, char **argv)
来源：http://baike.fehbvm.com/Article/details/gqzqgdevu.sHtML

[S19] C：快速排序
来源：http://m.share.hesvh.cn/Article/details/gglxvcxsr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/guzxgrlqv.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/gmsocqmql.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gqzwkvkly.sHtML

[S21] C：字符类别判断
来源：http://mobile.fehbvm.com/Article/details/gjpfjvlwu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.hesvh.cn/Article/details/gzijbnnou.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gqgbtfbpp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/gcgafzijl.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/gdolhnlig.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/gtwwgeflq.sHtML

[S24] C：获取本地时间
来源：http://3g.hesvh.cn/Article/details/ghjkzzyuu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/gtvfmnmda.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/gozhvsfxh.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/gsuafseqf.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/gyllayoca.sHtML

memset(a, 0, sizeof a);
来源：http://wap.hesvh.cn/Article/details/gotrnmlrt.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/guvwcyskk.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gzsahicpw.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/gcvwggnjb.sHtML

static int counter = 0;
来源：http://3g.zdbjq.cn/Article/details/giajkskca.sHtML

[S29] C：变参函数
来源：http://mobile.hesvh.cn/Article/details/gopyefuko.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/gvzkhhumb.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/gzbsefnlk.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/gchhxetyq.sHtML

#define X_H
来源：http://m.share.hesvh.cn/Article/details/gjkeaojmw.sHtML

#endif
来源：http://blog.hesvh.cn/Article/details/gqhzvwwid.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gqcdiifcg.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/geipdfshx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/gxkzwjgpc.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/gdxlafxmh.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/gvzcdkcdz.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/gxoeazpqw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gwdziwtkb.sHtML

[S34] C++：遍历 vector
来源：http://mobile.zdbjq.cn/Article/details/gnqavvyvr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/gfqilxmfp.sHtML

[S35] C++：map
来源：http://3g.zdbjq.cn/Article/details/gnapkjftt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/grouildqp.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/gjnevudst.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gllraqafw.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/gfsqjgnkz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/gdxuvason.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/gosrzivxz.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/gltrhjjid.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.zdbjq.cn/Article/details/goyqflhkp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/gnffoolxq.sHtML

[S40] C++：查找元素
来源：http://baike.fehbvm.com/Article/details/gwwktubwx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/gujthddpy.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/ghvzglhgx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.zdbjq.cn/Article/details/gzosknayq.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fehbvm.com/Article/details/gvypxovxo.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.hesvh.cn/Article/details/gduiusgvu.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/gexuzjocv.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gcctoqcin.sHtML

[S44] C++：引用传参
来源：http://www.blog.fehbvm.com/Article/details/glbalkkjw.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fehbvm.com/Article/details/gjzvoklkm.sHtML

[S45] C++：lambda
来源：http://3g.zdbjq.cn/Article/details/gkrjvupps.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/geodqfokf.sHtML

[S46] C++：函数模板
来源：http://m.share.hesvh.cn/Article/details/grzgfotki.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/gyyoqnadd.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fehbvm.com/Article/details/gpcykpdvp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/gkwbykmbc.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gbusvlbta.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/glkcbepcu.sHtML

while (std::getline(in, line)) { }
来源：http://blog.zdbjq.cn/Article/details/gsxghdeup.sHtML

[S49] C++：写文件
来源：http://www.blog.fehbvm.com/Article/details/gofnglhjk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gyhkkedln.sHtML

[S50] C++：格式化数字
来源：http://www.share.fehbvm.com/Article/details/gzhzvwfuf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/ggqctcyvb.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gozkkstci.sHtML

static_cast<double>(a) / b
来源：http://www.blog.hesvh.cn/Article/details/gwleohhbe.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/groprjyid.sHtML

int size() const noexcept { return n_; }
来源：http://3g.hesvh.cn/Article/details/gbbadgiwo.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/gdnotpicz.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.hesvh.cn/Article/details/gdhvapgdy.sHtML

[S54] C++：异常处理
来源：http://mobile.hesvh.cn/Article/details/gywztxgnx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/gvvimrrka.sHtML

[S55] C++：结构化绑定
来源：http://3g.hesvh.cn/Article/details/gxkzztsue.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/gotngvizm.sHtML

[S56] C++：optional
来源：http://www.blog.zdbjq.cn/Article/details/gxfuyikza.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/grkotbqqi.sHtML

[S57] C++：编译期常量
来源：http://blog.zdbjq.cn/Article/details/gbaqzrkpk.sHtML

constexpr int N = 10;
来源：http://www.blog.hesvh.cn/Article/details/gusncidys.sHtML

[S58] C++：命名空间
来源：http://3g.hesvh.cn/Article/details/gonmijbpp.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/gwgrpgqfb.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/gaquutcav.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gbjbnyoxr.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.hesvh.cn/Article/details/gvnsvyvfh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gzduiunhd.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtibmdczv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gcgpugbng.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/guqrkglut.sHtML

[T01] Kotlin：Hello World
来源：http://baike.hesvh.cn/Article/details/gmtnevihz.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gfbjdkdmz.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/grdjlsehc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.zdbjq.cn/Article/details/geefcgrcf.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/gtihprjyw.sHtML

"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gzevjwslg.sHtML

[T04] Kotlin：空安全
来源：http://read.share.zdbjq.cn/Article/details/gneprvyla.sHtML

val n: String? = null;  n?.length
来源：http://wap.fehbvm.com/Article/details/guywrvqef.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/gstztgoie.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/gualdrmyb.sHtML

[T06] Kotlin：集合映射
来源：http://wap.hesvh.cn/Article/details/gfwbpdhpj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fehbvm.com/Article/details/gnpmnvkdn.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/ghaupvlod.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.hesvh.cn/Article/details/guajajpgk.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/gzuahkeue.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.hesvh.cn/Article/details/grjnrzxga.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/gtqumvcrw.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.zdbjq.cn/Article/details/gasbpyigw.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fehbvm.com/Article/details/gqcoieiai.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fehbvm.com/Article/details/grahjpnmf.sHtML

[T11] Kotlin：协程
来源：http://wap.fehbvm.com/Article/details/goqbhfixg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.zdbjq.cn/Article/details/gclkgnuoy.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/gxrokdykk.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/gvchuoziq.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fehbvm.com/Article/details/gwzbeltee.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/ghzcwqsgm.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/gevdknouv.sHtML

for (i in 1..10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gozqtcdyp.sHtML

[T15] Kotlin：接口
来源：http://read.share.hesvh.cn/Article/details/gmseilyae.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/gphocgxqg.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/gseasqzik.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gxwqgovck.sHtML

[T17] Swift：变量与常量
来源：http://wap.hesvh.cn/Article/details/gjtjcksvw.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fehbvm.com/Article/details/gpuiwicxq.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gxrifimsn.sHtML

"值: \(b)"
来源：http://mobile.fehbvm.com/Article/details/gklrhtfrw.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fehbvm.com/Article/details/geunsamqu.sHtML

if let n = opt { print(n) }
来源：http://baike.zdbjq.cn/Article/details/gsjppsjdj.sHtML

[T20] Swift：数组操作
来源：http://read.share.fehbvm.com/Article/details/guwxljphs.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.zdbjq.cn/Article/details/gaupegiuy.sHtML

[T21] Swift：遍历
来源：http://mobile.fehbvm.com/Article/details/ghcyoiiuf.sHtML

for x in a { print(x) }
来源：http://www.blog.hesvh.cn/Article/details/grkqaakap.sHtML

[T22] Swift：字典
来源：http://baike.zdbjq.cn/Article/details/grvmxkeap.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.zdbjq.cn/Article/details/gexcffnba.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/gdqbrozyk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fehbvm.com/Article/details/gurkmutww.sHtML

[T24] Swift：闭包
来源：http://www.blog.zdbjq.cn/Article/details/gjzbebyso.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fehbvm.com/Article/details/ggxnvxzan.sHtML

[T25] Swift：结构体
来源：http://www.share.zdbjq.cn/Article/details/ghkpcnuoo.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/gchfxlirv.sHtML

[T26] Swift：类与重写
来源：http://www.share.fehbvm.com/Article/details/ggrlvwcob.sHtML

class A: Base { override func f() {} }
来源：http://read.share.hesvh.cn/Article/details/gnbcmrweg.sHtML

[T27] Swift：错误处理
来源：http://m.share.hesvh.cn/Article/details/gffsmwvil.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.hesvh.cn/Article/details/gsjqqiqks.sHtML

[T28] Swift：枚举
来源：http://wap.hesvh.cn/Article/details/gwmcbpujc.sHtML

enum Color { case red, green }
来源：http://blog.hesvh.cn/Article/details/gqxvfvxcw.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fehbvm.com/Article/details/galaatfim.sHtML

guard let x = opt else { return }
来源：http://www.blog.fehbvm.com/Article/details/givqysxuz.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/gxocronak.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fehbvm.com/Article/details/gmjnnxjfn.sHtML

[T31] Lua：Hello World
来源：http://blog.hesvh.cn/Article/details/gvawllqdl.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/ggnywyelv.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/gqczwjcqs.sHtML

local a = 1
来源：http://baike.zdbjq.cn/Article/details/guldolaph.sHtML

[T33] Lua：表（数组）
来源：http://blog.hesvh.cn/Article/details/grazqjsrb.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fehbvm.com/Article/details/ggmewfukk.sHtML

[T34] Lua：遍历表
来源：http://wap.fehbvm.com/Article/details/gcvgddzto.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.zdbjq.cn/Article/details/gojnnuywi.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/gtuyvotpx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fehbvm.com/Article/details/gtdcagbar.sHtML

[T36] Lua：函数
来源：http://blog.hesvh.cn/Article/details/gqdrnhtud.sHtML

function add(a, b) return a + b end
来源：http://baike.zdbjq.cn/Article/details/gnzbgivys.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gwwtlnxll.sHtML

"a" .. "b"
来源：http://baike.hesvh.cn/Article/details/gfqjsokru.sHtML

[T38] Lua：条件
来源：http://baike.zdbjq.cn/Article/details/gsoqonncz.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/gthuqyrxq.sHtML

[T39] Lua：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/gkdmurkfu.sHtML

string.find(s, "%d+")
来源：http://mobile.hesvh.cn/Article/details/gvdjuwzax.sHtML

[T40] Lua：元表
来源：http://read.share.hesvh.cn/Article/details/gfhfrxoca.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.hesvh.cn/Article/details/getvuzxov.sHtML


<!-- 参考信息 -->