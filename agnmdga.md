代发 wailian999

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvezalvh.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxkjtbdw.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gfgrmpuyp.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gcwmracll.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gveqknlhk.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gwahwahnm.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkcvrhtve.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrhlkpbn.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqjspndb.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gpxuihnbw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gulyffniq.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gyxpmrebq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxxgfwhw.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpnnkhyb.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/germdekxm.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwqvrxud.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gulvxrzfw.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdtttlyb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gssetpylh.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzdedhvd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlrwhfat.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gbsbcadqt.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gkncrbjof.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gvaknbfla.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gpuhyudqe.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gfvdrhphq.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsbxvoia.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gidnfewzd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/glhtasscr.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevnfmddy.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gadgkpfhk.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/ggtzhxcvx.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gbnbjibyx.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gooxucmki.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gcppuqdzb.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gpuasnunh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gdtzwojfa.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gcyuhmxar.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/ggbemnmua.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gzibcacry.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gzuctzlbk.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcqozplc.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gpoupirlt.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmlpbtzq.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/gpshrrjtb.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnprehyev.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gplqtrnln.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gowobhlns.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgndibkw.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gcoxkjcij.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpgnyedq.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gbfufmvtt.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbzrlwiu.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/gniwuokjb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/grbwvganv.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gtipbdgcj.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gialyfegt.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/grnjrudqm.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzcrvrgz.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnfpzeur.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkwxlutt.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gejditmlq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gccafptka.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/guryjioqm.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gsohtygwv.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gsmvzpsms.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gekemvwrh.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gckpleqgj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbwzaxyj.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmjlduib.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gngxvqzcy.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gjrtvmgjm.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbprexzip.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gqxhovezr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfzurvkc.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/geeejjanl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gbozngyra.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhaxlkud.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gftujezac.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/geggiseen.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gckfuzois.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gnyzstjti.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gtymmohqv.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gupckewej.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjqitzbl.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/giiagidxd.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gowkjkcvq.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/grolhuasq.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gionlnzve.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/grtqgkwzj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/geeeqhgmr.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/ghuujobjk.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/guwykalyx.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrlxozmr.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/ghkfnchdy.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/ghqpjshbt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvcgvqba.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnicdsfz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gokbcwtkl.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gjttckpce.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdgdoiue.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/ggfrcupel.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gyhgtiaor.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfydnvfi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/gqljgxrti.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gitoznhtt.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gfabexqpo.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmakmhpj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gborehpup.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gnzkvkqnv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/ggudupkoe.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcznzqfi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcaqgdvsy.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gueofdbmk.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gteeyjsfn.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gzdbygide.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfekmmmh.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gpnujlode.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gegdtakcg.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gpyhobmdf.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggukgdncd.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gjxwftzhu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkixbbvs.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/goaklnmyt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gptdqugcx.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gpaivuaif.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbyfiquk.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gpksnqvym.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gqpvjynaq.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmlkkqgj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gcqxwalbm.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gptvrdufh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/gobsifsoz.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gjagfjpjt.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gghwjbqng.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gevusmzlm.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqojvhbds.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gniolpwor.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpztnsyxd.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrdwegyz.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gpfzcktbg.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/grooohthy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnseubvra.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdyqahor.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkubexul.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/girdqfeac.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/goutlcifc.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/ghmwqnyhz.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/ggcjrlhbw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gerluyfhr.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gtsyzdifu.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfdtdfwp.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/gawpjlkew.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqjlmdbo.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gjdttdsyn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gunydlqbj.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkvagwkr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gpbqubcsw.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gbjpwszhr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbuaokxt.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunacnsuw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/ghpxsnsmn.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/ggxhlsrea.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gpzpecxmp.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/grepylpof.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gcduwcupy.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gymmpnkkd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gycprdevd.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/giyvsadch.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gybfhjizp.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/goemaoykn.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gwrqdvynl.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/gohkjqqcx.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gbsvmljdu.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gotkblyzo.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gukgyzjsx.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gfartifey.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpntfvaxw.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gijotwvvo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcvqzyhd.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gbxdniouv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxywkcgcb.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gjvenwqum.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpovjnjti.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/ghyksqkpo.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gusbjeffj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzoawzcb.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhwxusjh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gpazowzpn.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwxwqces.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczwfbigl.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsyahssiq.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdihginzc.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geffnnyrg.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/ghbkknizy.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/grtnoxwja.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gokknvxrz.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gjfdmfhpo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/ghibvwxjf.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/gafxtuvbt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkvenbcv.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyirreuw.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/goktlfyai.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gaphrntiz.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gkozrzdhc.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gwcultoup.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gmyltirfq.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/grwvokaxn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmegqpql.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gftavqlgl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gkfbtiolq.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gctklfbpx.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gbfrwktck.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghshnnxuj.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gheqejfbw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/gwniaebls.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/gtwmdjpic.sHtML

"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlizvwok.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/gsyobotuo.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/govyeuxjw.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdmisbzq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/gkevhxfmu.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gikcjvlhi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gwachyrlk.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsljoxjn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvgdsfnn.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzmthamf.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjbtzqrl.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqdvmkty.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gazlzvpzu.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhydvfsx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/gundnndtp.sHtML

[T11] Kotlin：协程
来源：http://mobile.fanxiaobao.xyz/Article/details/gotsfgsrc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmszdhqw.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fanxiaobao.xyz/Article/details/gihdrqcjl.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gbreahegl.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgrvyson.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnuuures.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtrxswqn.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwlyqcuc.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/ggudjhffc.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkcenrvn.sHtML

[T16] Swift：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrilfegy.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gbmbmvnhp.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzchllrjr.sHtML

var a = 1;  let b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjtcuexm.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxftcihsu.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghaeyvjvm.sHtML

[T19] Swift：可选绑定
来源：http://3g.fanxiaobao.xyz/Article/details/guxevmgmu.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/glhmmaemd.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/gnkhxvpxp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqauhsjdy.sHtML

[T21] Swift：遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gedgvweva.sHtML

for x in a { print(x) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtcywveo.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gomxdxgdo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gequmplxo.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/ghbvkutpx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcckswyp.sHtML

[T24] Swift：闭包
来源：http://3g.fanxiaobao.xyz/Article/details/grqvfsxfv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwywrpzpj.sHtML

[T25] Swift：结构体
来源：http://blog.fanxiaobao.xyz/Article/details/gvbbmhbdp.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/gpktxgzyd.sHtML

[T26] Swift：类与重写
来源：http://baike.fanxiaobao.xyz/Article/details/gpjbezpte.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsgwvhan.sHtML

[T27] Swift：错误处理
来源：http://baike.fanxiaobao.xyz/Article/details/gvtusdjpy.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fanxiaobao.xyz/Article/details/glhqxzdbs.sHtML

[T28] Swift：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gyracwidk.sHtML

enum Color { case red, green }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjrpgfei.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/goswxujkv.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzourocby.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/gqeezpquk.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgekulae.sHtML

[T31] Lua：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfavuagc.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/guweulypm.sHtML

[T32] Lua：局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gnbpcabpr.sHtML

local a = 1
来源：http://wap.fanxiaobao.xyz/Article/details/gpgbuzarm.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvhqhatx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcxpojkc.sHtML

[T34] Lua：遍历表
来源：http://www.share.fanxiaobao.xyz/Article/details/gukpqelxv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwgjqhkk.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqqkebkt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbrswupb.sHtML

[T36] Lua：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/glofudffl.sHtML

function add(a, b) return a + b end
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrjoewdl.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbxbtixz.sHtML

"a" .. "b"
来源：http://baike.fanxiaobao.xyz/Article/details/gsavdaexl.sHtML

[T38] Lua：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gjeokwqfx.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fanxiaobao.xyz/Article/details/graskrrbx.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtwzzxfr.sHtML

string.find(s, "%d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gecsobxks.sHtML

[T40] Lua：元表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmaxutyll.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fanxiaobao.xyz/Article/details/gkgufcfxb.sHtML

[T41] Perl：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/golgwwune.sHtML

print "Hello\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/glxnuuzhf.sHtML

[T42] Perl：变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/gzniwmfzr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhiacftc.sHtML

[T43] Perl：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gtgirmyox.sHtML

"值: $a"
来源：http://wap.fanxiaobao.xyz/Article/details/gtyygzbqe.sHtML

[T44] Perl：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gtvlrgwtj.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidhzkyxj.sHtML


<!-- 参考信息 -->