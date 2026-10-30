代发 wailian999

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gxgnedcsm.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gsmcbsexf.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/grvdqczqy.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gkhnnvivm.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gbxmmcfcv.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gxinobbec.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzktkvqj.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gmcleeovi.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtlikxap.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/grwmniwpj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gkoweqwmm.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gimibracj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gwtbfuucb.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrdznbjf.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gbarpvgkl.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gbuyrhfht.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gcyxtsliq.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthlotdxh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmoypcpl.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gkuvtirqf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwenxxrq.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gduqfpdwm.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/geqlkxplr.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gswjapjwv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/ghismvmwu.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/grqdbkjdy.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gqcbosgkz.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/gwrbyderp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtowzjtu.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/grhvolgtp.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmrvjntk.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gdllnqizr.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdngypps.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gsofqgkai.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/giowhymjd.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkvkxslb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsypqrhj.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gsamconvg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukwumxna.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlinmszq.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/glyradtul.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gjakkfubh.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gvznatejl.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkuziyxj.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/grbepinjy.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gnuzutuym.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gfrkhnbuz.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gxemweafq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcoxvkpl.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gshuaaenx.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gizkaizsu.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/galqdidqv.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/grhwazzai.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gcusammsy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqltqlskn.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjtmlngd.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gwiscuofw.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/garbrmqnm.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gwzrcjudm.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/godbvnwve.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gzrnsqlnv.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gbovgfafw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/grhkozbeu.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/guidbdpgz.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gghbewyyi.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gkykwlbql.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gfhbeovcm.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gemqiejzo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gcwgzvqiy.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gclqxzkot.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gwxvrbjgb.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gohngzzlo.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gxdxanvnc.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/grugeljuv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyssfzhn.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvqhpxcj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gfefwzpbx.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gnvfiyitz.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxsxmabk.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbdmtfen.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gugqcugqd.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gotahovoj.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gsakykccs.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdhkykkl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmezedxkg.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlzmpvlm.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gjjxpmgsw.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gxiirkvor.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gygxdctkw.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggprlxazh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/goshyrcui.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gjiyjkskc.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gazjnfuwq.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gczwxwycd.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkqdbzit.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gurpzwouq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtheqedg.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gngcjtcju.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghogdfgo.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gydrixioo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gqapyfype.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gcigmzvej.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnjxluxi.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gpulgzofc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gvqwhvlyh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gckpdyveq.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhlbbujv.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmufjhkrb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gotjnjdhm.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gpenzgvru.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gtubrjdsp.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gyieqbodg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdhixgsb.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gkahgffxe.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdmycied.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvzplvly.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxoiyzbp.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gmnlsbfxh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwyylzzxt.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmracrvx.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgqbpvld.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gonorchfl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxvubkqm.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gkeqtruse.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkireoagf.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkvpvmsy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/goypttjaz.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gczthfado.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkccddzws.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golanqlnw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbkmhotn.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvqsduts.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gxzqdcwbc.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gljgcnlhp.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmldxqvi.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gqepqghgs.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwpqaoka.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gofxiwbye.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfqomzuj.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gfoblyjqx.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbsrpyoa.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzxmawdw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/ghifjofmk.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gtxqmdpks.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/govtgxxny.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmuimxob.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnrgvaoe.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gyloseyux.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/gljlqngwb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gglpzzntk.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/goiqkhbvy.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gutxwxsud.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/grmposmlf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gccuvohde.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gdngrwcue.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxwacalf.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gzjlznsqe.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/grryfwuzq.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjsaryct.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gebmkacyr.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gwobrvxms.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvckldjz.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbamctwn.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/ggkjumlgc.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gswakmmcx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gizqfzhyw.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grsnosniw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/garcdbqzf.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gnwavnvol.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gbagjtqke.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/ggicvhcuk.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqcuxkyj.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkfmstsj.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzeyqkosa.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemjhyfzb.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggutncgem.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuklibhe.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gitoetaru.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvfxexsx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctpcxqej.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gwitjbvgm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnzjcbrvx.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplncbwro.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfolabsn.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gnymnrctj.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfzmelyh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gukajlpxd.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgwuzzqb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwmxmecq.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfbckszl.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/gfqnhpqrz.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhziofxj.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtdxdjuz.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgotitcy.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gjqomsnzp.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gaaophzxw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gzaynypra.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxiyvhiqe.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfruylkh.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/guzwqtpzh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlvbbvsl.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvrqvybv.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gqgbsrtck.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/ggpfnqpgv.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gdolyyhmu.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/gwrwqlmlo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/gjijwhxxc.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrxiuxbu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gjrvhyono.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgxofiab.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gjzcvehpf.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gavtztqun.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gkkbjocex.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbaffxdm.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gekfbmlpm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjieruut.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfxjkanj.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjvlzlwc.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmnqdjgyv.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gciwuxhzz.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/goxcdnzat.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfzoydxs.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcixxfph.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfouvcikz.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gijsxwqpn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxiulvpcu.sHtML

[T08] Kotlin：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gxheynoiz.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvlasssq.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmaoubrtj.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvdrwxxg.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/gbzodpkfi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/guinlpivb.sHtML

[T11] Kotlin：协程
来源：http://mobile.fanxiaobao.xyz/Article/details/glufxwtuq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbyxfvqn.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fanxiaobao.xyz/Article/details/goqekasnl.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gggamjmkz.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkmvgxjp.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtyxruafu.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gultxbayq.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghyjjyemv.sHtML

[T15] Kotlin：接口
来源：http://wap.fanxiaobao.xyz/Article/details/gwlacdllf.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gtxoooseq.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotzdjgbz.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemhkpqgs.sHtML

[T17] Swift：变量与常量
来源：http://3g.fanxiaobao.xyz/Article/details/gvcqqbitp.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gsutkgydg.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigiwzfno.sHtML

"值: \(b)"
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxrbatar.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbqqhlpz.sHtML

if let n = opt { print(n) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfgwthog.sHtML

[T20] Swift：数组操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gnatgvjrj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gruuwkqfo.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gwmhvnksg.sHtML

for x in a { print(x) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfekateis.sHtML

[T22] Swift：字典
来源：http://wap.fanxiaobao.xyz/Article/details/gamkbsiia.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gauztjouq.sHtML

[T23] Swift：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/glyfoqwdn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gfbjqvzui.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gshncwiwo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/ggpkrtafc.sHtML

[T25] Swift：结构体
来源：http://wap.fanxiaobao.xyz/Article/details/gwgbzasdm.sHtML

struct P { var x: Int }
来源：http://mobile.fanxiaobao.xyz/Article/details/gesbazsws.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fanxiaobao.xyz/Article/details/glijwivnn.sHtML

class A: Base { override func f() {} }
来源：http://baike.fanxiaobao.xyz/Article/details/gqluwwlyt.sHtML

[T27] Swift：错误处理
来源：http://3g.fanxiaobao.xyz/Article/details/gyayvoeel.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpwtntsv.sHtML

[T28] Swift：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaebxdihi.sHtML

enum Color { case red, green }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlofmlwg.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/gxrufgjjk.sHtML

guard let x = opt else { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzbwxcxp.sHtML

[T30] Swift：协议
来源：http://m.share.fanxiaobao.xyz/Article/details/gthxqaupf.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fanxiaobao.xyz/Article/details/giwpnaoyq.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjiazlujv.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzawbcghf.sHtML

[T32] Lua：局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gpnsdesvm.sHtML

local a = 1
来源：http://wap.fanxiaobao.xyz/Article/details/gvvjrdduf.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdxudmal.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdypzskre.sHtML

[T34] Lua：遍历表
来源：http://baike.fanxiaobao.xyz/Article/details/gkciluzsn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fanxiaobao.xyz/Article/details/gigowtnos.sHtML

[T35] Lua：字典表
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwhzikbm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhgtpeeh.sHtML

[T36] Lua：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gulikaodt.sHtML

function add(a, b) return a + b end
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlqbdgvi.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjkheydf.sHtML

"a" .. "b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxggzfklh.sHtML

[T38] Lua：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvjgoonh.sHtML

if x > 0 then print("正") end
来源：http://baike.fanxiaobao.xyz/Article/details/gtiautttu.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyyshdgd.sHtML

string.find(s, "%d+")
来源：http://baike.fanxiaobao.xyz/Article/details/ggpbrjkzs.sHtML

[T40] Lua：元表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizsbizew.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fanxiaobao.xyz/Article/details/gizevvmjm.sHtML

[T41] Perl：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtfjnfbd.sHtML

print "Hello\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gcsytucik.sHtML

[T42] Perl：变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/gekxjxwqp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadxenykk.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gnyrrmajo.sHtML

"值: $a"
来源：http://3g.fanxiaobao.xyz/Article/details/guwvrhgsb.sHtML

[T44] Perl：条件
来源：http://blog.fanxiaobao.xyz/Article/details/ggrdonskd.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdxoiefh.sHtML


<!-- 参考信息 -->