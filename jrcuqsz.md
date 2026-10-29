代发 wailian999

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/gnjfxrkwf.sHtML

[R38] 管道串联
来源：http://read.share.hesvh.cn/Article/details/gjinctezx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/gnwqhpspe.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.hesvh.cn/Article/details/gffnihdjh.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/gssrokmqm.sHtML

[R40] 追加写日志
来源：http://www.share.hesvh.cn/Article/details/grkfjivet.sHtML

echo "log" >> out.log
来源：http://www.m.share.hesvh.cn/Article/details/gxhahidjb.sHtML

[R41] 丢弃输出
来源：http://read.share.zdbjq.cn/Article/details/gbisgcxfx.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fehbvm.com/Article/details/gokvyjwhn.sHtML

[R42] 输入重定向
来源：http://www.share.fehbvm.com/Article/details/gpsffulvp.sHtML

wc -l < a.txt
来源：http://baike.zdbjq.cn/Article/details/gjuhfxvvi.sHtML

[R43] 按名字查找文件
来源：http://blog.fehbvm.com/Article/details/gxqtrsjcj.sHtML

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/gcuxlqrur.sHtML

[R44] 按修改时间查找
来源：http://m.share.hesvh.cn/Article/details/goyqrkdts.sHtML

find . -mtime -7 -type f
来源：http://mobile.zdbjq.cn/Article/details/gwmrabque.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/grwydyjkl.sHtML

find . -name "*.tmp" -delete
来源：http://wap.hesvh.cn/Article/details/gyxxwfdhe.sHtML

[R46] 递归替换文件内容
来源：http://www.share.zdbjq.cn/Article/details/gpnfekpjn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/gwtvtozsn.sHtML

[R47] sed 单行替换
来源：http://baike.fehbvm.com/Article/details/gvieakyhu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fehbvm.com/Article/details/gtesdsacc.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gxeguapys.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gwcgqkkze.sHtML

[R49] awk 带条件
来源：http://www.blog.zdbjq.cn/Article/details/gwviktioj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/gfdbiqswh.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/gfiuzlkvg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.hesvh.cn/Article/details/ggxqrdcvn.sHtML

[R51] 排序去重取前几
来源：http://baike.hesvh.cn/Article/details/giwrdekcz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.hesvh.cn/Article/details/gavqsxcww.sHtML

[R52] 统计行数
来源：http://mobile.fehbvm.com/Article/details/gqkyqmmlx.sHtML

wc -l a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gdxzwzely.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/gszeibutu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/gpdwnfppq.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/gppycfzwc.sHtML

diff a.txt b.txt
来源：http://wap.fehbvm.com/Article/details/gomzgerpv.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/gglchpqff.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/gwtybdrtf.sHtML

[R56] 远程拷贝
来源：http://m.share.hesvh.cn/Article/details/gpsiegzli.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/gomssoefd.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gkdvgbkch.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/gjibnpwgn.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/gzjvjejzh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/gqwctnwae.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/giicscito.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gdyeytpit.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gxleksgpp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/ggbqyqhex.sHtML

[R61] 磁盘占用
来源：http://read.share.zdbjq.cn/Article/details/gnupyatmu.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/gokfiecle.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/gillwhvjo.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.hesvh.cn/Article/details/gttwtgwyx.sHtML

[R63] 内存与进程
来源：http://mobile.zdbjq.cn/Article/details/gikmfczir.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/ggmtxidcg.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/gjxzuugvf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/gcdorpcpg.sHtML

[R65] 查看端口占用
来源：http://www.blog.hesvh.cn/Article/details/gpffhvzia.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.hesvh.cn/Article/details/gzzptfppy.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/gcpgxychy.sHtML

crontab -e;  crontab -l
来源：http://read.share.hesvh.cn/Article/details/gyuocixkp.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gomprcwbo.sHtML

openssl rand -hex 16
来源：http://m.share.fehbvm.com/Article/details/gxlnrkqwx.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/gcxtlnrrw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fehbvm.com/Article/details/gysepqhfm.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/gzdixdxxi.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/gbalheeqo.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/gpznwbzur.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/gjtteydua.sHtML

[R71] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gywulonvv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/gcbdexqtc.sHtML

[R72] 等待端口就绪
来源：http://wap.hesvh.cn/Article/details/gknxrjnzi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gofrogyze.sHtML

[R73] 分割大日志
来源：http://baike.zdbjq.cn/Article/details/gghzqoeeb.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/geonjosdo.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/gokyykpyk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/gqnkdvdzk.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/gltdxqysy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.zdbjq.cn/Article/details/gsqlfpyet.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/gcgasptng.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gqrowspxo.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/gciuvjyga.sHtML

read -rp "请输入: " ans
来源：http://baike.hesvh.cn/Article/details/gohfmxjrl.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/gnxupmcxa.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fehbvm.com/Article/details/gjwtvzxpr.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/gqvdtmrvo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/gysuvlzfl.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/gbjlyeamu.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/gesexqdjj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvhkhmyyd.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/gyvjihnrb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/golcugjdc.sHtML

[S01] C：Hello World
来源：http://m.share.hesvh.cn/Article/details/govscfiue.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/gdwdluqdn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.zdbjq.cn/Article/details/gorfcwjjx.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/grnjgrueq.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/ggoieoasg.sHtML

[S03] C：读入整数
来源：http://mobile.hesvh.cn/Article/details/gneplbzju.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/gtbltzhtq.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/grbjqtpem.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gcaidgmyf.sHtML

[S05] C：字符串长度
来源：http://3g.hesvh.cn/Article/details/ggudskvph.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/gsvffepgf.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gxbbltoum.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/gmraqdokc.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/gljdybvwv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fehbvm.com/Article/details/gisrgwhbo.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/gizzetmdq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.zdbjq.cn/Article/details/gbphrihje.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.hesvh.cn/Article/details/ganhlnfqo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.hesvh.cn/Article/details/gwbvxybic.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/gmpgxtuvu.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/gsqyylokt.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gezgptwuo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.zdbjq.cn/Article/details/gwfhthsiv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.zdbjq.cn/Article/details/gpiaxwszq.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/glgzilkpw.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gpojcwafp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gentmtnsh.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/gbnupahzh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/gsfrhdrku.sHtML

[S14] C：枚举
来源：http://mobile.fehbvm.com/Article/details/glzqgtpgv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fehbvm.com/Article/details/glhybukvl.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/gspajbdyf.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/gvbdbmiyw.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/gbjetgrml.sHtML

x |= (1 << 3);
来源：http://mobile.zdbjq.cn/Article/details/gjmmoxfui.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gksrcdxbg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gmvdckxye.sHtML

[S18] C：命令行参数
来源：http://mobile.hesvh.cn/Article/details/gwlvonoil.sHtML

int main(int argc, char **argv)
来源：http://read.share.zdbjq.cn/Article/details/gcqudbdvk.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/gwlwvreyz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/geqieziba.sHtML

[S20] C：二分查找
来源：http://m.share.fehbvm.com/Article/details/gpnfqvols.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gxzypanss.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/gnxkolomt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/gciorutkn.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/grqvsawez.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.zdbjq.cn/Article/details/ghfvqxnfj.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/gbnadyuha.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.zdbjq.cn/Article/details/grspeecgo.sHtML

[S24] C：获取本地时间
来源：http://read.share.fehbvm.com/Article/details/gyfynpyhr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.zdbjq.cn/Article/details/ggxdjtuzl.sHtML

[S25] C：内存拷贝
来源：http://www.blog.hesvh.cn/Article/details/geamuvayu.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.zdbjq.cn/Article/details/ggalfvdix.sHtML

[S26] C：内存清零
来源：http://baike.hesvh.cn/Article/details/gyohqpari.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/gcqnzhgax.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/gaozhdeav.sHtML

const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gqwnovlft.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/ghhjjzmoz.sHtML

static int counter = 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gvkbgrrcb.sHtML

[S29] C：变参函数
来源：http://mobile.fehbvm.com/Article/details/glhkypmhz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/gzqahjxrg.sHtML

[S30] C：头文件保护
来源：http://blog.zdbjq.cn/Article/details/gmpekgygl.sHtML

#ifndef X_H
来源：http://3g.hesvh.cn/Article/details/gepwsounk.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gcofrvbry.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/ggwsgfajy.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/gwhwxawso.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/gtezrzirg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fehbvm.com/Article/details/guuosnnwg.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/gwgxjcmbd.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/gqfbtcosv.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/gtmecxdig.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fehbvm.com/Article/details/gzyuwjnvm.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/gdpnaryml.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/gcqbxnrkz.sHtML

[S35] C++：map
来源：http://m.share.zdbjq.cn/Article/details/gwupmrlne.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/glgvrmufn.sHtML

[S36] C++：unordered_map
来源：http://mobile.zdbjq.cn/Article/details/gedvuempp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gxtsnahos.sHtML

[S37] C++：set
来源：http://www.share.fehbvm.com/Article/details/gwncynwdj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/gsjjifvbn.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/gwatsvsdz.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fehbvm.com/Article/details/gdoiiekxt.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.zdbjq.cn/Article/details/gsbwskfbm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gpyygqfvs.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/gzwmdgaua.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fehbvm.com/Article/details/gtciavamy.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fehbvm.com/Article/details/ggbyycymz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gaqqcddux.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fehbvm.com/Article/details/gnfgkpdli.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/gbcefxloh.sHtML

[S43] C++：智能指针
来源：http://www.share.hesvh.cn/Article/details/gbjnopoif.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.zdbjq.cn/Article/details/gukxkftwj.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/grvoorage.sHtML

void inc(int &x) { ++x; }
来源：http://wap.hesvh.cn/Article/details/gkyuajogg.sHtML

[S45] C++：lambda
来源：http://wap.hesvh.cn/Article/details/guiwlabbl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/gvhpdzntu.sHtML

[S46] C++：函数模板
来源：http://3g.zdbjq.cn/Article/details/gyoiaytmm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.hesvh.cn/Article/details/gxszkgmdu.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/gmcrmeqdh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fehbvm.com/Article/details/gqamrewkz.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gxkntqlqy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fehbvm.com/Article/details/gnqmqyaee.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gwrkwuoli.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/gynhcxqcv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.zdbjq.cn/Article/details/gcetkjxlx.sHtML

[S50] C++：格式化数字
来源：http://baike.fehbvm.com/Article/details/ghcvyztxk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fehbvm.com/Article/details/gjgkoadhx.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/gyudlesmc.sHtML

static_cast<double>(a) / b
来源：http://mobile.zdbjq.cn/Article/details/gxolhkuni.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.hesvh.cn/Article/details/glqsixapk.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/gpikazoku.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/gqwhehsmw.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.zdbjq.cn/Article/details/gdewjkdai.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/gyhmysipu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.zdbjq.cn/Article/details/gvtgjtntu.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/gkuzenueo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/gzonaptnh.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/gxagibwnr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.hesvh.cn/Article/details/gibaqtgwv.sHtML

[S57] C++：编译期常量
来源：http://blog.zdbjq.cn/Article/details/guudbkukl.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gxginzgnl.sHtML

[S58] C++：命名空间
来源：http://3g.fehbvm.com/Article/details/gdgzyelyg.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fehbvm.com/Article/details/gjuhfqpiy.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/gavqeeyhn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/gkqoxgcnp.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/gdelmlcqh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/gbzrnhdxu.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gzaqgtvgc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/gujpepocg.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gblbtwffg.sHtML

[T01] Kotlin：Hello World
来源：http://3g.hesvh.cn/Article/details/ghuudgmpf.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gjoggkfpd.sHtML

[T02] Kotlin：变量
来源：http://wap.fehbvm.com/Article/details/gfnxmcrtb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gzxhcyjaj.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.zdbjq.cn/Article/details/gdbrfgwqz.sHtML

"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gosfobmmz.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gofgydzhl.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/gxqetrwqq.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.hesvh.cn/Article/details/gwcjvpczk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/gcvbtsccj.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gcztgkrjq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gmqtexbwd.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/glzzjmynn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/gmbbbuizd.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/golkmjrnb.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gotsmewim.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/gxksjgfff.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.zdbjq.cn/Article/details/gfdefwhyo.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/gwgzcckkx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.zdbjq.cn/Article/details/gadryslpl.sHtML

[T11] Kotlin：协程
来源：http://mobile.fehbvm.com/Article/details/gsxqkbtaj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/getupcjvw.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/ghwxmzlwj.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gqypdswzi.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/guehvdbxn.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fehbvm.com/Article/details/ghynqnsis.sHtML

[T14] Kotlin：循环
来源：http://m.share.fehbvm.com/Article/details/gysgxvdgo.sHtML

for (i in 1..10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gbaomdqcd.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.zdbjq.cn/Article/details/gzhaubxkk.sHtML

interface Shape { fun area(): Double }
来源：http://blog.hesvh.cn/Article/details/geogvfaod.sHtML

[T16] Swift：Hello World
来源：http://wap.zdbjq.cn/Article/details/gwnytxjad.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gcfsyxccv.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/gnqwmgpcc.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gbexrherw.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gvhrcscru.sHtML

"值: \(b)"
来源：http://baike.fehbvm.com/Article/details/gjtjbjrpq.sHtML

[T19] Swift：可选绑定
来源：http://read.share.zdbjq.cn/Article/details/gnywhejyq.sHtML

if let n = opt { print(n) }
来源：http://wap.zdbjq.cn/Article/details/gooianlxa.sHtML

[T20] Swift：数组操作
来源：http://blog.zdbjq.cn/Article/details/gtphupzix.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/gxiumbnex.sHtML

[T21] Swift：遍历
来源：http://read.share.fehbvm.com/Article/details/gvyafrbns.sHtML

for x in a { print(x) }
来源：http://wap.fehbvm.com/Article/details/ghqhqihgn.sHtML

[T22] Swift：字典
来源：http://www.m.share.fehbvm.com/Article/details/gvamvnubr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.hesvh.cn/Article/details/gyzplmzga.sHtML

[T23] Swift：函数
来源：http://blog.zdbjq.cn/Article/details/ggvusidmk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/gvokmhktp.sHtML

[T24] Swift：闭包
来源：http://www.blog.zdbjq.cn/Article/details/gbmajijmg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gidajnhrw.sHtML

[T25] Swift：结构体
来源：http://3g.zdbjq.cn/Article/details/gsjkrzykg.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/glncnqvxa.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/gknodtjps.sHtML

class A: Base { override func f() {} }
来源：http://m.share.zdbjq.cn/Article/details/gjfuzxudn.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/gigauyupg.sHtML

do { try f() } catch { print(error) }
来源：http://wap.hesvh.cn/Article/details/gtpmwicrh.sHtML

[T28] Swift：枚举
来源：http://3g.fehbvm.com/Article/details/gjpfuwwyi.sHtML

enum Color { case red, green }
来源：http://www.m.share.fehbvm.com/Article/details/gtkpeftqy.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fehbvm.com/Article/details/gzcpoxewi.sHtML

guard let x = opt else { return }
来源：http://m.share.hesvh.cn/Article/details/gxtibjebo.sHtML

[T30] Swift：协议
来源：http://www.blog.fehbvm.com/Article/details/gwpknuwsm.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.hesvh.cn/Article/details/ghyqyaitq.sHtML

[T31] Lua：Hello World
来源：http://baike.fehbvm.com/Article/details/gzbyqcijg.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/geprpznvh.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fehbvm.com/Article/details/gesxqktuz.sHtML

local a = 1
来源：http://wap.zdbjq.cn/Article/details/gkdqfknxn.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fehbvm.com/Article/details/gecmcvspb.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.hesvh.cn/Article/details/gpuotbnfx.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/gmcuzofig.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.zdbjq.cn/Article/details/gupxwcvjw.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/gdatnkfaj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.hesvh.cn/Article/details/gdsozorig.sHtML

[T36] Lua：函数
来源：http://blog.hesvh.cn/Article/details/gvklseflu.sHtML

function add(a, b) return a + b end
来源：http://3g.hesvh.cn/Article/details/gxyhytdid.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gqlexdcpz.sHtML

"a" .. "b"
来源：http://m.share.zdbjq.cn/Article/details/ggmjvllsv.sHtML

[T38] Lua：条件
来源：http://www.share.hesvh.cn/Article/details/gfdwsrzzs.sHtML

if x > 0 then print("正") end
来源：http://blog.fehbvm.com/Article/details/gxiuzyaiy.sHtML

[T39] Lua：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gcvghntci.sHtML

string.find(s, "%d+")
来源：http://read.share.zdbjq.cn/Article/details/grtpugewh.sHtML

[T40] Lua：元表
来源：http://3g.hesvh.cn/Article/details/ghpcyqglq.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fehbvm.com/Article/details/gtegnifeh.sHtML


<!-- 参考信息 -->