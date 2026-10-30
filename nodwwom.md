代发 wailian999

cmd > out.log 2>&1
来源：http://m.share.hesvh.cn/Article/details/gmwfpszvi.sHtML

[R40] 追加写日志
来源：http://www.blog.zdbjq.cn/Article/details/gzrkeebwu.sHtML

echo "log" >> out.log
来源：http://www.m.share.hesvh.cn/Article/details/ggvfnurvz.sHtML

[R41] 丢弃输出
来源：http://www.blog.hesvh.cn/Article/details/gsubgosfi.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.zdbjq.cn/Article/details/grsilpoen.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/giizfntlb.sHtML

wc -l < a.txt
来源：http://m.share.zdbjq.cn/Article/details/gtcepqvqx.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/gbapocjmv.sHtML

find . -name "*.log" -type f
来源：http://mobile.zdbjq.cn/Article/details/gahiexzib.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/gffomsbwx.sHtML

find . -mtime -7 -type f
来源：http://m.share.hesvh.cn/Article/details/glcgemvkn.sHtML

[R45] 批量删除
来源：http://read.share.fehbvm.com/Article/details/gymsggwdr.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/gefpifmgw.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fehbvm.com/Article/details/gotmkscjb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/gurublezw.sHtML

[R47] sed 单行替换
来源：http://baike.fehbvm.com/Article/details/gcxadhmgs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/giodowqmo.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/ghdoxpwkf.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.hesvh.cn/Article/details/glruzbfqj.sHtML

[R49] awk 带条件
来源：http://blog.fehbvm.com/Article/details/gdgmqnenn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.zdbjq.cn/Article/details/gocwfuhdo.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/gimxbvfjs.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gshyipmfd.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/gjspvlyhc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fehbvm.com/Article/details/gmcnzpier.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/gtyrecvbs.sHtML

wc -l a.txt
来源：http://www.share.fehbvm.com/Article/details/ghflyixnp.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.zdbjq.cn/Article/details/gidisudpl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fehbvm.com/Article/details/gkbuwoebc.sHtML

[R54] 比较两个文件
来源：http://wap.zdbjq.cn/Article/details/gskeffqss.sHtML

diff a.txt b.txt
来源：http://baike.fehbvm.com/Article/details/ghxkauoja.sHtML

[R55] 压缩与解压
来源：http://mobile.fehbvm.com/Article/details/gtkwvygdr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fehbvm.com/Article/details/gmdxtjyls.sHtML

[R56] 远程拷贝
来源：http://3g.fehbvm.com/Article/details/gasixoxvz.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/gokkktkhd.sHtML

[R57] 远程执行命令
来源：http://blog.fehbvm.com/Article/details/gbtmctieq.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/guqmgkysw.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/gogipgdqq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fehbvm.com/Article/details/gwuvpafqj.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gwvxtwese.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/guehowyft.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gljjwaujj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/gpkquuonp.sHtML

[R61] 磁盘占用
来源：http://3g.fehbvm.com/Article/details/gnqdgbswk.sHtML

df -h;  du -sh *
来源：http://m.share.fehbvm.com/Article/details/gwowkqrgo.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/glbtrioux.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gtnjtdhev.sHtML

[R63] 内存与进程
来源：http://mobile.zdbjq.cn/Article/details/gofikpttt.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/gkjblxoaj.sHtML

[R64] 结束进程
来源：http://read.share.fehbvm.com/Article/details/gsvtlizke.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/gjadfbldy.sHtML

[R65] 查看端口占用
来源：http://www.share.zdbjq.cn/Article/details/ggwlfhkaq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.zdbjq.cn/Article/details/gcrpjtxmu.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/gsyixmrbf.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/gextflwpg.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/ggghlppnb.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/gcfmveegn.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/gtqznecnp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gswvffdyq.sHtML

[R69] 生成随机密码
来源：http://www.blog.fehbvm.com/Article/details/gpqwzwrov.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/gmmnyqcny.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/ghrgpyxdv.sHtML

date +%s;  date -d @1700000000
来源：http://wap.zdbjq.cn/Article/details/guxtjzynq.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gaumziudp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fehbvm.com/Article/details/grzipmtuc.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/girrgwqgk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gxpkhvvhb.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/geatkkhuv.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/gsmgtadnx.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/gvlfhpoju.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/ggqyfdzbh.sHtML

[R75] 导出环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gsjcifoxu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/gebqbricb.sHtML

[R76] 使用临时文件
来源：http://3g.hesvh.cn/Article/details/gmreexfxc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gamtodund.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/gxcruxkez.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/ggarzmsmd.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/gbittfumj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.zdbjq.cn/Article/details/gqcyquutv.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/grfczafur.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.hesvh.cn/Article/details/gjquuvnfa.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.hesvh.cn/Article/details/gbklsecsp.sHtML

time ./run.sh
来源：http://read.share.fehbvm.com/Article/details/gupeoacws.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/guidlcrps.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/gjwoovssa.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbezigzej.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gkiyojjwc.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/gapsraeod.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/gdalssvwb.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fehbvm.com/Article/details/gabykyvpb.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/guvvapaen.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/gtzqrquxo.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/gqhdfokfm.sHtML

[S04] C：字符串复制
来源：http://m.share.zdbjq.cn/Article/details/gipwmjtzp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fehbvm.com/Article/details/gmudevuay.sHtML

[S05] C：字符串长度
来源：http://baike.zdbjq.cn/Article/details/gaqhpacbz.sHtML

strlen(s)
来源：http://m.share.zdbjq.cn/Article/details/geykomqdg.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/gyrdpfwow.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/ghvydafou.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/gywvbmoue.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/gzvaduxdc.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/gvbxmlpmf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.zdbjq.cn/Article/details/gxoakxnqb.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/gwczyjnjj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/ghrubhpmi.sHtML

[S10] C：指针与解引用
来源：http://blog.zdbjq.cn/Article/details/gagzmvtnn.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.zdbjq.cn/Article/details/gsebxwofy.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/ghhnixqct.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.hesvh.cn/Article/details/gqrpoluhl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fehbvm.com/Article/details/guptdioho.sHtML

fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gouivtwkb.sHtML

[S12] C：写文件
来源：http://mobile.fehbvm.com/Article/details/gqgcwjmak.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gawweocrc.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/gktdoackw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.hesvh.cn/Article/details/gwvrbpwze.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/gnkqybzut.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/gfdgtswqg.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/gygakmvci.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/gpjuwhsnt.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/gyafloqnx.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/gmcmlbozi.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fehbvm.com/Article/details/gaobfujsd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fehbvm.com/Article/details/glqayfgxy.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/gzfkemfph.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/gdmxlltca.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/glkusgsbu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gelvnpdyq.sHtML

[S20] C：二分查找
来源：http://wap.fehbvm.com/Article/details/gvykaswij.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gebajmmvf.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/gecbxudnn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/gfqfxcico.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/gobkjpozm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/gbapihqxn.sHtML

[S23] C：随机数
来源：http://m.share.zdbjq.cn/Article/details/gtjgliptz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.zdbjq.cn/Article/details/gqipbaipf.sHtML

[S24] C：获取本地时间
来源：http://mobile.zdbjq.cn/Article/details/gquvsraml.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/gbdeflwwo.sHtML

[S25] C：内存拷贝
来源：http://m.share.hesvh.cn/Article/details/gmxbxoadq.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/guyabeydm.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/genzrasht.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.hesvh.cn/Article/details/glzszjosb.sHtML

[S27] C：定义常量
来源：http://blog.zdbjq.cn/Article/details/gakvzfoht.sHtML

const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/grzazafbc.sHtML

[S28] C：静态变量
来源：http://m.share.fehbvm.com/Article/details/gyxhhhdce.sHtML

static int counter = 0;
来源：http://www.share.hesvh.cn/Article/details/gffkeopae.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/gtbxycauh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.hesvh.cn/Article/details/gapwpxmoc.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/gugkcxoeu.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/gzqrcjglo.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gsuspcbdp.sHtML

#endif
来源：http://m.share.fehbvm.com/Article/details/gbbjusmam.sHtML

[S31] C++：Hello World
来源：http://m.share.hesvh.cn/Article/details/gpfroqmcg.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/ghrxiaoyw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/gvmctwzlx.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/guxgdawyb.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/gdifvmpwt.sHtML

[S33] C++：vector 增删
来源：http://www.share.hesvh.cn/Article/details/gptmkrwdx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.zdbjq.cn/Article/details/gvlslxqgx.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/gdadpwncn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fehbvm.com/Article/details/gqwetylsr.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/gftpwqpne.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gojrlaiqc.sHtML

[S36] C++：unordered_map
来源：http://3g.fehbvm.com/Article/details/gszwdasgd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gbqonlrbr.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/giigxrfyd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/gdiczgasq.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/gsomlaslg.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/ghmbpndjx.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fehbvm.com/Article/details/gyencilfn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fehbvm.com/Article/details/ghpkxcbaf.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/gfwhtrthr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.hesvh.cn/Article/details/gxougpqaf.sHtML

[S41] C++：类与构造函数
来源：http://m.share.zdbjq.cn/Article/details/gcschchwx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.zdbjq.cn/Article/details/gortdbuod.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/gseuoljub.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/gidyxslrq.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/guttzftsm.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/gavialmoj.sHtML

[S44] C++：引用传参
来源：http://www.share.fehbvm.com/Article/details/gnvzbzdve.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/gujainbnd.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/gysyhopms.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.hesvh.cn/Article/details/givdrrwqy.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/gqdmaaiiv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/grzfrcuzy.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.zdbjq.cn/Article/details/gbadbdebh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.zdbjq.cn/Article/details/gsbbpftfp.sHtML

[S48] C++：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gakoqhuws.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fehbvm.com/Article/details/ggzcubsmx.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/gtidffriu.sHtML

[S49] C++：写文件
来源：http://wap.fehbvm.com/Article/details/grmzcwhlo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/gkzwvfyhw.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gfgoazrey.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/ggnmdmcpw.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fehbvm.com/Article/details/gapwbvmae.sHtML

static_cast<double>(a) / b
来源：http://m.share.hesvh.cn/Article/details/gjorhiyze.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.zdbjq.cn/Article/details/ghofkfpdd.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.hesvh.cn/Article/details/gkdzxjuxw.sHtML

[S53] C++：移动语义
来源：http://mobile.fehbvm.com/Article/details/gtltvuaef.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fehbvm.com/Article/details/gzvxipucs.sHtML

[S54] C++：异常处理
来源：http://blog.hesvh.cn/Article/details/giwfdrrmd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fehbvm.com/Article/details/gqujcshdv.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/gilycndva.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/gutpjscck.sHtML

[S56] C++：optional
来源：http://baike.zdbjq.cn/Article/details/geufmgkxy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/gpmgitrvl.sHtML

[S57] C++：编译期常量
来源：http://3g.zdbjq.cn/Article/details/gwvsnkgjd.sHtML

constexpr int N = 10;
来源：http://3g.zdbjq.cn/Article/details/ggbvsinev.sHtML

[S58] C++：命名空间
来源：http://3g.zdbjq.cn/Article/details/gxlshxzws.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fehbvm.com/Article/details/gjymvizpm.sHtML

[S59] C++：静态断言
来源：http://baike.hesvh.cn/Article/details/gpsgwjkcq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.zdbjq.cn/Article/details/gkiporagb.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.hesvh.cn/Article/details/gmfggnloe.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gcjkcvxxt.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfwoqhjno.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/gzpuopenm.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxbglcgdz.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gmhxzqsax.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/grxyuxjrn.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/gdbonzubf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/gewyiklqx.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/gbyumirjc.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/gskcfowoz.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fehbvm.com/Article/details/gulbaiwkk.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fehbvm.com/Article/details/guobszzme.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/gczqcuclp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/gdphggzpf.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/gfkruuooz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/gqndvjgzl.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gpnbfuqai.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.hesvh.cn/Article/details/gyugxhebe.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/gtykpibfz.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gfwikgxff.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/guacdhkjr.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fehbvm.com/Article/details/gaopmkfez.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fehbvm.com/Article/details/gglkjubta.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.zdbjq.cn/Article/details/grvxowbsp.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/grpqvvmde.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/gpjulteok.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.zdbjq.cn/Article/details/gkbmzmqgu.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gigvnihpg.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.hesvh.cn/Article/details/grnmubsay.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fehbvm.com/Article/details/gmwhnvyig.sHtML

[T14] Kotlin：循环
来源：http://read.share.hesvh.cn/Article/details/gvjifoqpd.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fehbvm.com/Article/details/glstlxmlz.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/gcrjmyuuk.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.zdbjq.cn/Article/details/gvxsikhts.sHtML

[T16] Swift：Hello World
来源：http://mobile.hesvh.cn/Article/details/gwrsirjiy.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gdwfblfhg.sHtML

[T17] Swift：变量与常量
来源：http://blog.zdbjq.cn/Article/details/geomsjhxj.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/gvpucghng.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gjhqyjcce.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/gikncoimf.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/gpiembxdm.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/gaqiylllk.sHtML

[T20] Swift：数组操作
来源：http://blog.fehbvm.com/Article/details/gayegabar.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.hesvh.cn/Article/details/grkkciulk.sHtML

[T21] Swift：遍历
来源：http://3g.zdbjq.cn/Article/details/gyeeokjrl.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/grpeivenw.sHtML

[T22] Swift：字典
来源：http://www.m.share.fehbvm.com/Article/details/gomyjhjlo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.zdbjq.cn/Article/details/geweraxnn.sHtML

[T23] Swift：函数
来源：http://wap.zdbjq.cn/Article/details/gyrpdajgb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.zdbjq.cn/Article/details/gzxaiwxlh.sHtML

[T24] Swift：闭包
来源：http://www.share.zdbjq.cn/Article/details/goqokogac.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gxczklbdv.sHtML

[T25] Swift：结构体
来源：http://www.blog.fehbvm.com/Article/details/gqbtsnfhm.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/gmqebmgzv.sHtML

[T26] Swift：类与重写
来源：http://blog.fehbvm.com/Article/details/gspkzpqdm.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/ghpfsxhcp.sHtML

[T27] Swift：错误处理
来源：http://baike.zdbjq.cn/Article/details/gcaywnxpg.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fehbvm.com/Article/details/glekeyaaw.sHtML

[T28] Swift：枚举
来源：http://wap.hesvh.cn/Article/details/ggfxirpcf.sHtML

enum Color { case red, green }
来源：http://wap.fehbvm.com/Article/details/gvdayxnfj.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fehbvm.com/Article/details/gpxxccozr.sHtML

guard let x = opt else { return }
来源：http://wap.hesvh.cn/Article/details/gdiuoehrs.sHtML

[T30] Swift：协议
来源：http://www.share.fehbvm.com/Article/details/gwgeqiwer.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.zdbjq.cn/Article/details/gssxlyuuo.sHtML

[T31] Lua：Hello World
来源：http://baike.zdbjq.cn/Article/details/gvxmwbyhn.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gibrwuwul.sHtML

[T32] Lua：局部变量
来源：http://wap.zdbjq.cn/Article/details/gmogfsazl.sHtML

local a = 1
来源：http://wap.hesvh.cn/Article/details/gomehyjtb.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.zdbjq.cn/Article/details/guttfvjpw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fehbvm.com/Article/details/gkwssvrkv.sHtML

[T34] Lua：遍历表
来源：http://blog.hesvh.cn/Article/details/gtdygfpce.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.hesvh.cn/Article/details/gzeuqvfuk.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/goqxcgiin.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.hesvh.cn/Article/details/ghtmdsljl.sHtML

[T36] Lua：函数
来源：http://wap.zdbjq.cn/Article/details/gdyeqaumu.sHtML

function add(a, b) return a + b end
来源：http://blog.hesvh.cn/Article/details/gyebuupvp.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gdldlapnh.sHtML

"a" .. "b"
来源：http://www.m.share.hesvh.cn/Article/details/gyxrbzsyl.sHtML

[T38] Lua：条件
来源：http://www.m.share.hesvh.cn/Article/details/glzxrilhr.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.zdbjq.cn/Article/details/gvrggqlgw.sHtML

[T39] Lua：模式匹配
来源：http://blog.zdbjq.cn/Article/details/ggknxqezz.sHtML

string.find(s, "%d+")
来源：http://www.share.fehbvm.com/Article/details/guskxxobu.sHtML

[T40] Lua：元表
来源：http://www.share.fehbvm.com/Article/details/gsjxvwysm.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.hesvh.cn/Article/details/gofqkkzpg.sHtML

[T41] Perl：Hello World
来源：http://blog.zdbjq.cn/Article/details/gsttzdona.sHtML

print "Hello\n";
来源：http://mobile.hesvh.cn/Article/details/ghwnybhsn.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.zdbjq.cn/Article/details/gdzsouvhw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.hesvh.cn/Article/details/gyrkczgdr.sHtML


<!-- 参考信息 -->