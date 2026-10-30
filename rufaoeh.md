代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/gxapjxuxe.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/gcfkamvaz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/ghgmvdzch.sHtML

[R37] 把输出赋给变量
来源：http://baike.zdbjq.cn/Article/details/gtphulwth.sHtML

files=$(ls -1)
来源：http://wap.fehbvm.com/Article/details/gvnfqhlfr.sHtML

[R38] 管道串联
来源：http://www.share.zdbjq.cn/Article/details/gaksajtre.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/gxrtzfhno.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.hesvh.cn/Article/details/gptqbvnqn.sHtML

cmd > out.log 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gmayjmvvj.sHtML

[R40] 追加写日志
来源：http://3g.fehbvm.com/Article/details/gghpevlba.sHtML

echo "log" >> out.log
来源：http://m.share.fehbvm.com/Article/details/gcmlnkydz.sHtML

[R41] 丢弃输出
来源：http://mobile.fehbvm.com/Article/details/giotkbxna.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/gusbudkes.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/gbmqqddkf.sHtML

wc -l < a.txt
来源：http://www.m.share.hesvh.cn/Article/details/grjyydydc.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/gaywvhpku.sHtML

find . -name "*.log" -type f
来源：http://baike.fehbvm.com/Article/details/gzrmjkqaw.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/gjoygudmb.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/gksfgmnns.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/gdgfvhmur.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.hesvh.cn/Article/details/gkgabbnwy.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fehbvm.com/Article/details/grapbhpbk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.zdbjq.cn/Article/details/gmqitepfx.sHtML

[R47] sed 单行替换
来源：http://blog.hesvh.cn/Article/details/goafkvuvy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/gspmeclra.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/gavbtwrzn.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gqtsnojeo.sHtML

[R49] awk 带条件
来源：http://www.share.zdbjq.cn/Article/details/gqewlxmhy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/grolhfgqo.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/gkptunmbu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/ggyskrbiv.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/gvhneekai.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/gsilonjfz.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/gptdxxufv.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/guqywgbgc.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/gpzwidttu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/gbmssbliy.sHtML

[R54] 比较两个文件
来源：http://wap.fehbvm.com/Article/details/gbaohsxhp.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/ggproajmg.sHtML

[R55] 压缩与解压
来源：http://m.share.zdbjq.cn/Article/details/gdzeovozw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.hesvh.cn/Article/details/gtgmtfpki.sHtML

[R56] 远程拷贝
来源：http://read.share.fehbvm.com/Article/details/gsjbjkswb.sHtML

scp file user@host:/path/
来源：http://mobile.fehbvm.com/Article/details/gpcsfgcbr.sHtML

[R57] 远程执行命令
来源：http://www.blog.fehbvm.com/Article/details/gedlibllx.sHtML

ssh user@host 'uptime'
来源：http://blog.hesvh.cn/Article/details/gzlxdtvhi.sHtML

[R58] 下载文件
来源：http://baike.hesvh.cn/Article/details/gucmolrho.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.zdbjq.cn/Article/details/gjriuxrci.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/gwlmraxkg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.zdbjq.cn/Article/details/gzhpeunet.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/ggidscflq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gfaeaslry.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/gucfjyjxt.sHtML

df -h;  du -sh *
来源：http://baike.zdbjq.cn/Article/details/gzdalgwer.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/geijvbown.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.hesvh.cn/Article/details/gkebmbdvn.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/gnuftoqlj.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/gfpdkwhcw.sHtML

[R64] 结束进程
来源：http://3g.hesvh.cn/Article/details/gthkgfcyp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/gepvqwhon.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/gyvradyqd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/gbtqfyuzm.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/gqxqqtott.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/gvrcoptcs.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.zdbjq.cn/Article/details/gqmorenti.sHtML

openssl rand -hex 16
来源：http://blog.zdbjq.cn/Article/details/grbvoygsu.sHtML

[R68] 计算文件校验值
来源：http://3g.zdbjq.cn/Article/details/gmwyfvamo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/gnjdiaczg.sHtML

[R69] 生成随机密码
来源：http://blog.hesvh.cn/Article/details/gxduhbneg.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/gaizgrrtf.sHtML

[R70] 时间戳与互转
来源：http://www.blog.zdbjq.cn/Article/details/gipkwnkzx.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.hesvh.cn/Article/details/gtlcrcjab.sHtML

[R71] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gnyalsesd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/gdzzzuovh.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/guscekvrk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gshzkkqbl.sHtML

[R73] 分割大日志
来源：http://baike.zdbjq.cn/Article/details/gmafzahnh.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/gbaywjecx.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/gktalkiyp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/gkwxucnny.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gyllqjffs.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/gdvdolpal.sHtML

[R76] 使用临时文件
来源：http://www.share.fehbvm.com/Article/details/glgbezrbj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gamnxpgdy.sHtML

[R77] 读取用户输入
来源：http://read.share.zdbjq.cn/Article/details/gsmyjgsgq.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gmtlqkwiz.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/grgcqqgtl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fehbvm.com/Article/details/gnfgzkqyr.sHtML

[R79] 解析命令行选项
来源：http://read.share.zdbjq.cn/Article/details/gkmbjratw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/gxjdyqlhb.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/gcovpijoe.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/gdsszcvpe.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnfjjwnhy.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/gtvtdzsea.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmclaoijc.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/gujafxqex.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/gpsbqiscs.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.hesvh.cn/Article/details/gefbcnmmi.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gblktjtew.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gvhivjlit.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/gywwryfbb.sHtML

int x; scanf("%d", &x);
来源：http://www.share.zdbjq.cn/Article/details/gnebzqbzw.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gdsupvsau.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/ghwjnlhnw.sHtML

[S05] C：字符串长度
来源：http://blog.hesvh.cn/Article/details/gslupfcja.sHtML

strlen(s)
来源：http://baike.fehbvm.com/Article/details/gtupmqfms.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/gqmhxfhzc.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/gtmzkqzon.sHtML

[S07] C：数组遍历求和
来源：http://read.share.hesvh.cn/Article/details/gywmjlgio.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/gmmfktnfd.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.hesvh.cn/Article/details/gtqavztjo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/gshgnfbcc.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.hesvh.cn/Article/details/gqmedmjxp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/gckmlyaro.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/grsgbuwux.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/goukrjqqu.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gjmemrrdh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.zdbjq.cn/Article/details/gmhbxgzcu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.hesvh.cn/Article/details/gajoprtmw.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gopiqghoe.sHtML

[S12] C：写文件
来源：http://blog.hesvh.cn/Article/details/gxirxpvhm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gjfnpuxoz.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/gwbprvhla.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/gmpsfkypp.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/gjldakdqe.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.hesvh.cn/Article/details/gtmlcghkx.sHtML

[S15] C：类型转换
来源：http://mobile.zdbjq.cn/Article/details/gunczftxs.sHtML

(double) a / b
来源：http://3g.hesvh.cn/Article/details/getbxfxyx.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/gkgmabjwu.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/gtsakhxjb.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fehbvm.com/Article/details/grkrfrpcl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gvlsromrv.sHtML

[S18] C：命令行参数
来源：http://read.share.hesvh.cn/Article/details/gehbgvfqt.sHtML

int main(int argc, char **argv)
来源：http://m.share.zdbjq.cn/Article/details/gayxqkfzl.sHtML

[S19] C：快速排序
来源：http://www.share.fehbvm.com/Article/details/gcubfakxz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gssraqssb.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/gscaodnfq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/grvboxfbg.sHtML

[S21] C：字符类别判断
来源：http://3g.zdbjq.cn/Article/details/gqouvwxpc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/gmlqrurcg.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gfahxzunt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fehbvm.com/Article/details/gpfttwrrj.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/gptbejpkc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/gorcaoeai.sHtML

[S24] C：获取本地时间
来源：http://baike.fehbvm.com/Article/details/gnmwivgsh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.zdbjq.cn/Article/details/gnshmfroh.sHtML

[S25] C：内存拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gjvtehpgs.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gtxaumzzu.sHtML

[S26] C：内存清零
来源：http://wap.hesvh.cn/Article/details/ggmgvcrqw.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fehbvm.com/Article/details/gdpofjcup.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/gqohamqtj.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gnlbyuuds.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/gmzestquf.sHtML

static int counter = 0;
来源：http://baike.zdbjq.cn/Article/details/gwfqwcksf.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/gweldlffh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/gkajkrymo.sHtML

[S30] C：头文件保护
来源：http://mobile.zdbjq.cn/Article/details/gxplpjsgj.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/gpxicqdib.sHtML

#define X_H
来源：http://mobile.hesvh.cn/Article/details/ggaqedeal.sHtML

#endif
来源：http://m.share.hesvh.cn/Article/details/gejfmrhxl.sHtML

[S31] C++：Hello World
来源：http://wap.fehbvm.com/Article/details/gyyenozvb.sHtML

#include <iostream>
来源：http://www.blog.hesvh.cn/Article/details/gvsgkboqr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/glyrpijcb.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/gdndvdchz.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.hesvh.cn/Article/details/gebkhefgo.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/gcivbertf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/gtmdgpzee.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/goafozakh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/gstbdlqad.sHtML

[S35] C++：map
来源：http://baike.fehbvm.com/Article/details/guzeomthb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gqhspfftc.sHtML

[S36] C++：unordered_map
来源：http://www.share.fehbvm.com/Article/details/gqxvtlehm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gimfqkzzj.sHtML

[S37] C++：set
来源：http://baike.zdbjq.cn/Article/details/guibxbndz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/gfyrofwhq.sHtML

[S38] C++：排序
来源：http://www.blog.zdbjq.cn/Article/details/givnmsgco.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fehbvm.com/Article/details/gfbsbmvlm.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.hesvh.cn/Article/details/gwizzrtdx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.hesvh.cn/Article/details/gcmxvlpdd.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/gbkleqkkj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/gkelelrss.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/gheottpkl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/gopecsxgu.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/gdzklrnev.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/gjltnfmjc.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/gkrvusvyj.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fehbvm.com/Article/details/guzxlytyp.sHtML

[S44] C++：引用传参
来源：http://m.share.zdbjq.cn/Article/details/gsqrhdyec.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fehbvm.com/Article/details/goglbeffz.sHtML

[S45] C++：lambda
来源：http://baike.hesvh.cn/Article/details/gkpelmeea.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/giglaccut.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gjcassokm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.hesvh.cn/Article/details/gdzrymlek.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fehbvm.com/Article/details/gfqhwdbxu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fehbvm.com/Article/details/gcdsexcjk.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gtysjmczs.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/gvzbzeiti.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gbuunwidn.sHtML

[S49] C++：写文件
来源：http://www.blog.hesvh.cn/Article/details/gbizutvxw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gmzgjhivj.sHtML

[S50] C++：格式化数字
来源：http://www.share.hesvh.cn/Article/details/gemlzlkur.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gpczxcwqq.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fehbvm.com/Article/details/ggzdjfvdb.sHtML

static_cast<double>(a) / b
来源：http://wap.zdbjq.cn/Article/details/gqbrppjlv.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/gwyursqna.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.zdbjq.cn/Article/details/gidxxbyvb.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/ggibqszst.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.hesvh.cn/Article/details/gwbvcduws.sHtML

[S54] C++：异常处理
来源：http://mobile.zdbjq.cn/Article/details/gdginrkgg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/geyvbxzhd.sHtML

[S55] C++：结构化绑定
来源：http://baike.zdbjq.cn/Article/details/grfxqilyw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.zdbjq.cn/Article/details/ggcuflhpg.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/gvhuvwkia.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.hesvh.cn/Article/details/gnatyqxhy.sHtML

[S57] C++：编译期常量
来源：http://blog.zdbjq.cn/Article/details/gyfwymkhc.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/gbpexevqv.sHtML

[S58] C++：命名空间
来源：http://read.share.fehbvm.com/Article/details/gdoppvpsr.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/ghaexzxmy.sHtML

[S59] C++：静态断言
来源：http://www.m.share.zdbjq.cn/Article/details/guibmmkpk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.zdbjq.cn/Article/details/guujpijnc.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.zdbjq.cn/Article/details/gjbpfnmpz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.hesvh.cn/Article/details/gsgtnkmao.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdkochbfn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gecbvmtbt.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grrmxstnf.sHtML

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/gzijdrais.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gaxfmmzlu.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fehbvm.com/Article/details/gcwyyzpni.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fehbvm.com/Article/details/gptmclncc.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.hesvh.cn/Article/details/gxkiexwzh.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gsfwgbwtk.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/gxtxabpyq.sHtML

val n: String? = null;  n?.length
来源：http://www.share.hesvh.cn/Article/details/gujliiqwh.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/ggqwdkbmz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/gtaljdrii.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gphpuzqsg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.zdbjq.cn/Article/details/gzzehqaqe.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gdvgpbwer.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/gawjpfbjp.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/gzsexxhrr.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/gsycmzikf.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.zdbjq.cn/Article/details/gsoseiizl.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fehbvm.com/Article/details/gffgbbmot.sHtML

[T10] Kotlin：默认参数
来源：http://wap.zdbjq.cn/Article/details/gcagxoclf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.hesvh.cn/Article/details/guhlkrpnw.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gvlbkpgac.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/gjtiefdoe.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.zdbjq.cn/Article/details/gnoqmwbdu.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/ghirudfwf.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/gsakfhvsw.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fehbvm.com/Article/details/grvxitqdd.sHtML

[T14] Kotlin：循环
来源：http://read.share.zdbjq.cn/Article/details/gbbpgmwsy.sHtML

for (i in 1..10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gxegokydf.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fehbvm.com/Article/details/gawpgtpnx.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fehbvm.com/Article/details/gpqinzwhd.sHtML

[T16] Swift：Hello World
来源：http://wap.fehbvm.com/Article/details/gqywtpznm.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gsaerocdt.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.hesvh.cn/Article/details/gglsyfdub.sHtML

var a = 1;  let b = 2
来源：http://wap.fehbvm.com/Article/details/gpggziswj.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gtvfiqsoc.sHtML

"值: \(b)"
来源：http://baike.zdbjq.cn/Article/details/gzmekiujp.sHtML

[T19] Swift：可选绑定
来源：http://read.share.zdbjq.cn/Article/details/ggwaglbba.sHtML

if let n = opt { print(n) }
来源：http://3g.fehbvm.com/Article/details/gmilejdiv.sHtML

[T20] Swift：数组操作
来源：http://www.share.fehbvm.com/Article/details/gmyaqtgfw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.zdbjq.cn/Article/details/gxvgueazz.sHtML

[T21] Swift：遍历
来源：http://3g.hesvh.cn/Article/details/gxxzhidmc.sHtML

for x in a { print(x) }
来源：http://blog.fehbvm.com/Article/details/gjuvggzxh.sHtML

[T22] Swift：字典
来源：http://www.m.share.zdbjq.cn/Article/details/gqgasxpah.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.zdbjq.cn/Article/details/gwmyaxjon.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/gggwdcsjk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.hesvh.cn/Article/details/gjtvzjrkh.sHtML

[T24] Swift：闭包
来源：http://baike.hesvh.cn/Article/details/gubotltor.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/getrpqmfu.sHtML

[T25] Swift：结构体
来源：http://wap.fehbvm.com/Article/details/gwytnqncs.sHtML

struct P { var x: Int }
来源：http://mobile.fehbvm.com/Article/details/gnpgixwfa.sHtML

[T26] Swift：类与重写
来源：http://blog.zdbjq.cn/Article/details/geedwdxxy.sHtML

class A: Base { override func f() {} }
来源：http://wap.hesvh.cn/Article/details/gosnxlwvg.sHtML

[T27] Swift：错误处理
来源：http://3g.hesvh.cn/Article/details/gvncezbls.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fehbvm.com/Article/details/ghcyrtgwi.sHtML

[T28] Swift：枚举
来源：http://www.share.zdbjq.cn/Article/details/gqjlnevei.sHtML

enum Color { case red, green }
来源：http://3g.hesvh.cn/Article/details/gduflzqwl.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/gcelxwqgo.sHtML

guard let x = opt else { return }
来源：http://baike.hesvh.cn/Article/details/gfvlvpkjl.sHtML

[T30] Swift：协议
来源：http://3g.fehbvm.com/Article/details/gcbciuntw.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.zdbjq.cn/Article/details/gasrprlij.sHtML

[T31] Lua：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gqpjbufny.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gfyksvfih.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fehbvm.com/Article/details/gpggjlljy.sHtML

local a = 1
来源：http://blog.hesvh.cn/Article/details/gjcydbugp.sHtML

[T33] Lua：表（数组）
来源：http://baike.fehbvm.com/Article/details/gvohnyujq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/gnzcswqcy.sHtML

[T34] Lua：遍历表
来源：http://mobile.hesvh.cn/Article/details/gwgzbjexm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.hesvh.cn/Article/details/gsynmmxqu.sHtML

[T35] Lua：字典表
来源：http://read.share.hesvh.cn/Article/details/gsqenrscs.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fehbvm.com/Article/details/gjmmadmys.sHtML

[T36] Lua：函数
来源：http://m.share.fehbvm.com/Article/details/gvdweemex.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fehbvm.com/Article/details/gymgjiutu.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gnaetbnxg.sHtML

"a" .. "b"
来源：http://m.share.fehbvm.com/Article/details/ghqzuefai.sHtML

[T38] Lua：条件
来源：http://baike.fehbvm.com/Article/details/gefbrdnky.sHtML

if x > 0 then print("正") end
来源：http://www.blog.zdbjq.cn/Article/details/gugonqzrs.sHtML


<!-- 参考信息 -->