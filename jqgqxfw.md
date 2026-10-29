代发 wailian999

files=$(ls -1)
来源：http://www.blog.zdbjq.cn/Article/details/goqklbxxq.sHtML

[R38] 管道串联
来源：http://www.blog.fehbvm.com/Article/details/gihyespqy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fehbvm.com/Article/details/gqiebijrh.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/glkpvudlc.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/giijubppk.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/gpahzdbwr.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/gnjbujttq.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/gzlihduxx.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.zdbjq.cn/Article/details/ggetyvgfr.sHtML

[R42] 输入重定向
来源：http://wap.zdbjq.cn/Article/details/ggflwanre.sHtML

wc -l < a.txt
来源：http://wap.zdbjq.cn/Article/details/gmasftimm.sHtML

[R43] 按名字查找文件
来源：http://m.share.hesvh.cn/Article/details/gegvjzmqg.sHtML

find . -name "*.log" -type f
来源：http://www.share.hesvh.cn/Article/details/gljvvnaim.sHtML

[R44] 按修改时间查找
来源：http://3g.zdbjq.cn/Article/details/gqxguuazk.sHtML

find . -mtime -7 -type f
来源：http://www.blog.zdbjq.cn/Article/details/gknigeuku.sHtML

[R45] 批量删除
来源：http://m.share.fehbvm.com/Article/details/gsqiyejhi.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fehbvm.com/Article/details/glykwqktk.sHtML

[R46] 递归替换文件内容
来源：http://blog.zdbjq.cn/Article/details/gsdqggcuc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.zdbjq.cn/Article/details/glrhxfxaw.sHtML

[R47] sed 单行替换
来源：http://m.share.fehbvm.com/Article/details/gekkrhvzx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.zdbjq.cn/Article/details/grazqnwjp.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/gzggghfbe.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gwimabijv.sHtML

[R49] awk 带条件
来源：http://www.share.zdbjq.cn/Article/details/gfnknehai.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.hesvh.cn/Article/details/gjjytpiny.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/gyksmdhfc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/glmbsbdyc.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/giavpxdgl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.hesvh.cn/Article/details/gxntlzuvs.sHtML

[R52] 统计行数
来源：http://read.share.hesvh.cn/Article/details/gihmsmpmy.sHtML

wc -l a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gbmngbpfu.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.zdbjq.cn/Article/details/gorcqkilw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fehbvm.com/Article/details/gbuzbqwau.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/gowmvtvxh.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/gjsjomzrp.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/gvjrdnloe.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/golskhaug.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gxsfkvmvh.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/ghmhyizsa.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/guhoqilef.sHtML

ssh user@host 'uptime'
来源：http://m.share.hesvh.cn/Article/details/gsxoedybt.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/gjstgskff.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.zdbjq.cn/Article/details/gxiczdmmf.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/glzfsqowk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/gnpajvguz.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gqqpjzsfi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/giiwzswlp.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/gphsfcojr.sHtML

df -h;  du -sh *
来源：http://www.blog.hesvh.cn/Article/details/gsdjyzswc.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/goqweromi.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.zdbjq.cn/Article/details/gguqkfufj.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/ggtbkmybp.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/ghmipncof.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/gmpztfxid.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/gzubfgogz.sHtML

[R65] 查看端口占用
来源：http://wap.fehbvm.com/Article/details/gzntwyyed.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.zdbjq.cn/Article/details/gqdthxlui.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/gipeiioba.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/gxsejcgot.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fehbvm.com/Article/details/gegqqiwik.sHtML

openssl rand -hex 16
来源：http://mobile.zdbjq.cn/Article/details/gxdepizjp.sHtML

[R68] 计算文件校验值
来源：http://3g.hesvh.cn/Article/details/gvlacwsvj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gofaxsvfu.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/glpqlkgmt.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/ghgqcxkqt.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/gtepujzlq.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/gnlbrrium.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gojltqouu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/gklvmqist.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fehbvm.com/Article/details/gyczcmbng.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gjihfkqhu.sHtML

[R73] 分割大日志
来源：http://www.blog.fehbvm.com/Article/details/gqgyccfxq.sHtML

split -l 1000 big.log part_
来源：http://wap.fehbvm.com/Article/details/gqnlkzrhz.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gevyrqzui.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/gciakshnp.sHtML

[R75] 导出环境变量
来源：http://m.share.hesvh.cn/Article/details/gdgoppgfa.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/gmgirkybj.sHtML

[R76] 使用临时文件
来源：http://www.blog.hesvh.cn/Article/details/gpdxycqld.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/glafhwlcg.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/gqivyttri.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/ghxhfmvpi.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/gvbdkaemv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/gjljachbk.sHtML

[R79] 解析命令行选项
来源：http://3g.zdbjq.cn/Article/details/gzucepnok.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.hesvh.cn/Article/details/geiuatwxe.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/gebweguoq.sHtML

time ./run.sh
来源：http://www.share.hesvh.cn/Article/details/glrbkjaoa.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gorqhyjju.sHtML

S. C / C++ 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gqebgrhrh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/genusiutq.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/gwxsbwymn.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/gfmszzktn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gxmeiycny.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gozqtiqpl.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.hesvh.cn/Article/details/gjrewouue.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/gylehsdle.sHtML

int x; scanf("%d", &x);
来源：http://baike.fehbvm.com/Article/details/gumlraoog.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/gfvpehwux.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fehbvm.com/Article/details/gqtpgtojj.sHtML

[S05] C：字符串长度
来源：http://baike.fehbvm.com/Article/details/gesszotpq.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/gyrleltjf.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/gpircjudx.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/gjcbnjrqh.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/gfxuoguor.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fehbvm.com/Article/details/gfjipmjnf.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/grlkuhich.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/gcaggkxjm.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.hesvh.cn/Article/details/gjtoiwfxy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.hesvh.cn/Article/details/gyeylxfmn.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/gggsdkpvh.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/grngnucky.sHtML

[S11] C：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gkrpwxegi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/grqbzkcbk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fehbvm.com/Article/details/ggzkzpysa.sHtML

fclose(f);
来源：http://wap.hesvh.cn/Article/details/gehnfjoya.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/gbbbfinvb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.hesvh.cn/Article/details/gvjucawmk.sHtML

[S13] C：宏定义
来源：http://www.m.share.hesvh.cn/Article/details/gwquofpwa.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/gqgggvylf.sHtML

[S14] C：枚举
来源：http://3g.hesvh.cn/Article/details/gzhokkxuc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/giqvsbfjg.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/gtfodbacs.sHtML

(double) a / b
来源：http://m.share.fehbvm.com/Article/details/ghxtebmhh.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fehbvm.com/Article/details/glmvxzekw.sHtML

x |= (1 << 3);
来源：http://read.share.zdbjq.cn/Article/details/ggpqzswrg.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gwjyzbhyd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/gztlfylvi.sHtML

[S18] C：命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gfiklabqs.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/glgqegmmg.sHtML

[S19] C：快速排序
来源：http://m.share.zdbjq.cn/Article/details/gqbhexvkd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gbdlyorpq.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/gsyrslrwf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gzlajqern.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/glybxpyxp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/geavdbwvp.sHtML

[S22] C：字符串转数字
来源：http://mobile.fehbvm.com/Article/details/gczqaootw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/giatdrown.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/ggdcnebzi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gimavfjtk.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/gkkujqwth.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/govltimlm.sHtML

[S25] C：内存拷贝
来源：http://wap.zdbjq.cn/Article/details/goisfsypo.sHtML

memcpy(dst, src, n);
来源：http://www.share.zdbjq.cn/Article/details/gwxgruuvz.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/gxmhmokon.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/ggjfkikqm.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/goowbqlrp.sHtML

const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gosudjefb.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/gocwlsclu.sHtML

static int counter = 0;
来源：http://www.blog.fehbvm.com/Article/details/gmzwqmdfg.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/gtzmsgqoz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/gifqugnxb.sHtML

[S30] C：头文件保护
来源：http://3g.fehbvm.com/Article/details/ghwjjefdq.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/grhwhjdxn.sHtML

#define X_H
来源：http://mobile.zdbjq.cn/Article/details/gpvhejiik.sHtML

#endif
来源：http://www.m.share.hesvh.cn/Article/details/gqqrdknoy.sHtML

[S31] C++：Hello World
来源：http://baike.zdbjq.cn/Article/details/gvueuwpvm.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gfivvmanj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/gzsxilean.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/guqpxwggi.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/gusebwisy.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/gtxfewtvn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fehbvm.com/Article/details/gcdoeyrwo.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/gflrfstoj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.zdbjq.cn/Article/details/gpcaudfkv.sHtML

[S35] C++：map
来源：http://www.share.hesvh.cn/Article/details/gmvtxnfex.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gwncgihaq.sHtML

[S36] C++：unordered_map
来源：http://read.share.zdbjq.cn/Article/details/gszjoktxx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/ghydqaeof.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/goqzkxwnb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/giavbaqqi.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/gqqlgbico.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.hesvh.cn/Article/details/guyclofhg.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gcmjtmuje.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/gosgegkkr.sHtML

[S40] C++：查找元素
来源：http://3g.fehbvm.com/Article/details/gpydndrei.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.zdbjq.cn/Article/details/gruednbul.sHtML

[S41] C++：类与构造函数
来源：http://mobile.hesvh.cn/Article/details/gvztpnunw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/goptmevrs.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fehbvm.com/Article/details/girpsxpyy.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fehbvm.com/Article/details/gzlndwzbx.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/gyfzspnyz.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fehbvm.com/Article/details/gplnssgsu.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/gczyxxgxg.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/gwtiawzbp.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/gcynugwyx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/gbiaffsuq.sHtML

[S46] C++：函数模板
来源：http://mobile.fehbvm.com/Article/details/gxvlietye.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fehbvm.com/Article/details/gjylwlwya.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/gcsnqvhcw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/gyxnvclgg.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gqmlshkig.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.hesvh.cn/Article/details/gnakrpnue.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gbbaxnalp.sHtML

[S49] C++：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gntcrluiw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.zdbjq.cn/Article/details/gykbtwlyt.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/gdkrozizw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gwrmgzbhh.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fehbvm.com/Article/details/gkkfgizni.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/gjhbkfxev.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fehbvm.com/Article/details/gmitjwzgt.sHtML

int size() const noexcept { return n_; }
来源：http://wap.hesvh.cn/Article/details/gzjnjwcqc.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/goidjxmfi.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/guhrvblhq.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/gdquwbvfy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/gymblmjev.sHtML

[S55] C++：结构化绑定
来源：http://wap.zdbjq.cn/Article/details/guhppfvvu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.zdbjq.cn/Article/details/gjdlheurn.sHtML

[S56] C++：optional
来源：http://www.share.zdbjq.cn/Article/details/gymqpstcu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.hesvh.cn/Article/details/gsyystioq.sHtML

[S57] C++：编译期常量
来源：http://blog.zdbjq.cn/Article/details/geomdbech.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/gausbnzmd.sHtML

[S58] C++：命名空间
来源：http://read.share.fehbvm.com/Article/details/gnpwcdpmq.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.zdbjq.cn/Article/details/gbqonaczl.sHtML

[S59] C++：静态断言
来源：http://read.share.zdbjq.cn/Article/details/gjhvekfph.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.hesvh.cn/Article/details/gvwsygeiq.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/gkgtzvnmk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gbyarzowj.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gsqewhaiz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gmaladzjg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gdddoaefl.sHtML

[T01] Kotlin：Hello World
来源：http://wap.hesvh.cn/Article/details/gabuhtmeq.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gcamkdrcg.sHtML

[T02] Kotlin：变量
来源：http://www.share.fehbvm.com/Article/details/gnhrfsbun.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/grwkyhste.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.zdbjq.cn/Article/details/gsgxahics.sHtML

"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gnwfletyp.sHtML

[T04] Kotlin：空安全
来源：http://baike.zdbjq.cn/Article/details/gpxjeyyih.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/gqlduufhv.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gxjlojgip.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.zdbjq.cn/Article/details/gndmzysxi.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.hesvh.cn/Article/details/gnaxsnvja.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fehbvm.com/Article/details/gvfsfrmpq.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gsclcrfmo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.zdbjq.cn/Article/details/gdjpvdrpf.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/gjsvkhkyt.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fehbvm.com/Article/details/gsopxparf.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.zdbjq.cn/Article/details/gyedvrtdo.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.hesvh.cn/Article/details/gdmksofng.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fehbvm.com/Article/details/ghoaksvqq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.hesvh.cn/Article/details/gsiqxqcgg.sHtML

[T11] Kotlin：协程
来源：http://3g.fehbvm.com/Article/details/gvglcmctk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/gbdgfbzzk.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/gpvxpnfzh.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gajxrxtsu.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.zdbjq.cn/Article/details/ghvcepdma.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.zdbjq.cn/Article/details/gkzemrusx.sHtML

[T14] Kotlin：循环
来源：http://blog.hesvh.cn/Article/details/gvzihecxb.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gmwqylakg.sHtML

[T15] Kotlin：接口
来源：http://baike.fehbvm.com/Article/details/gdcqnpgbr.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.hesvh.cn/Article/details/ggqwfrctz.sHtML

[T16] Swift：Hello World
来源：http://blog.zdbjq.cn/Article/details/gtpnisvhq.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gmstcbtxb.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/gbibtvwdp.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/gkhrhgrxx.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gudylqgsz.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/gghddujig.sHtML

[T19] Swift：可选绑定
来源：http://baike.hesvh.cn/Article/details/gyarkvcto.sHtML

if let n = opt { print(n) }
来源：http://www.share.hesvh.cn/Article/details/gcfndjmjr.sHtML

[T20] Swift：数组操作
来源：http://blog.zdbjq.cn/Article/details/glcvnzllk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.hesvh.cn/Article/details/gpfbxzirw.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/gfeuxunth.sHtML

for x in a { print(x) }
来源：http://baike.fehbvm.com/Article/details/glpovaxmv.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/geyizabgh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.hesvh.cn/Article/details/gvqtmlauf.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/gbcwkwivt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.hesvh.cn/Article/details/gtwomodgm.sHtML

[T24] Swift：闭包
来源：http://blog.zdbjq.cn/Article/details/gclcimzqa.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gbjkhtydr.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/gcztgxacs.sHtML

struct P { var x: Int }
来源：http://www.blog.zdbjq.cn/Article/details/glrygcwes.sHtML

[T26] Swift：类与重写
来源：http://www.share.zdbjq.cn/Article/details/gpvefvjfo.sHtML

class A: Base { override func f() {} }
来源：http://m.share.hesvh.cn/Article/details/gizlkavet.sHtML

[T27] Swift：错误处理
来源：http://www.share.hesvh.cn/Article/details/grpfsrslo.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.zdbjq.cn/Article/details/ganaqmwgd.sHtML

[T28] Swift：枚举
来源：http://baike.zdbjq.cn/Article/details/gbwmnpttu.sHtML

enum Color { case red, green }
来源：http://read.share.hesvh.cn/Article/details/goicmsmxk.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fehbvm.com/Article/details/gcflpweew.sHtML

guard let x = opt else { return }
来源：http://wap.hesvh.cn/Article/details/gqghnygjl.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/gtozhepff.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fehbvm.com/Article/details/gocbdhgob.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/ggpwxtgtx.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gqisxowok.sHtML

[T32] Lua：局部变量
来源：http://wap.zdbjq.cn/Article/details/gtdpfyycn.sHtML

local a = 1
来源：http://www.share.zdbjq.cn/Article/details/gedfxkzvy.sHtML

[T33] Lua：表（数组）
来源：http://baike.hesvh.cn/Article/details/gmrxgqeqi.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.zdbjq.cn/Article/details/glhidnupo.sHtML

[T34] Lua：遍历表
来源：http://baike.zdbjq.cn/Article/details/gwhwrvsuv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fehbvm.com/Article/details/gjlrtvfsa.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/gvslnfeki.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.zdbjq.cn/Article/details/gkhwqajmo.sHtML

[T36] Lua：函数
来源：http://blog.hesvh.cn/Article/details/ggifhsefd.sHtML

function add(a, b) return a + b end
来源：http://m.share.hesvh.cn/Article/details/geihcliis.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/gzivqrfkq.sHtML

"a" .. "b"
来源：http://read.share.hesvh.cn/Article/details/grwvvmebr.sHtML

[T38] Lua：条件
来源：http://3g.hesvh.cn/Article/details/gkujhjidz.sHtML

if x > 0 then print("正") end
来源：http://wap.zdbjq.cn/Article/details/gofppowqu.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gfjmgfjea.sHtML

string.find(s, "%d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gftvazmet.sHtML

[T40] Lua：元表
来源：http://read.share.fehbvm.com/Article/details/gcmxxglkp.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.zdbjq.cn/Article/details/gsauankfb.sHtML


<!-- 参考信息 -->