代发 wailian999

files=$(ls -1)
来源：http://www.blog.zdbjq.cn/Article/details/goaqfdtxq.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/gvtfnxkuf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fehbvm.com/Article/details/gjenkyosj.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/gtxtytcuk.sHtML

cmd > out.log 2>&1
来源：http://www.share.fehbvm.com/Article/details/gumwtkoru.sHtML

[R40] 追加写日志
来源：http://www.blog.zdbjq.cn/Article/details/ghanebhky.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/gqtxtgixo.sHtML

[R41] 丢弃输出
来源：http://www.blog.fehbvm.com/Article/details/ghhtcnrng.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gyrtqfmpj.sHtML

[R42] 输入重定向
来源：http://blog.fehbvm.com/Article/details/glarkxadj.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/goouiiszw.sHtML

[R43] 按名字查找文件
来源：http://mobile.hesvh.cn/Article/details/gaxqzbefd.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/gxgkvowgk.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.hesvh.cn/Article/details/gmxkqeczg.sHtML

find . -mtime -7 -type f
来源：http://blog.zdbjq.cn/Article/details/gfvejvrrd.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/gasyexirl.sHtML

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/gkaxolwdh.sHtML

[R46] 递归替换文件内容
来源：http://m.share.hesvh.cn/Article/details/gzvxhpbzm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fehbvm.com/Article/details/gllbbhtxe.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/grmcxvkty.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fehbvm.com/Article/details/gwjwteicu.sHtML

[R48] awk 取指定列
来源：http://read.share.hesvh.cn/Article/details/gsqgkqpfo.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gzfwbtvym.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/gzhxizbic.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fehbvm.com/Article/details/gpnikrgyv.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/gcxnthpcj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gtaprlean.sHtML

[R51] 排序去重取前几
来源：http://mobile.hesvh.cn/Article/details/gujfzxcvf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/gnkxwgumy.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/geccvkhgj.sHtML

wc -l a.txt
来源：http://read.share.fehbvm.com/Article/details/ggslmjdjj.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/gkcalbtjo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fehbvm.com/Article/details/ghpathgss.sHtML

[R54] 比较两个文件
来源：http://blog.fehbvm.com/Article/details/gqxhfkjqz.sHtML

diff a.txt b.txt
来源：http://mobile.fehbvm.com/Article/details/gackncipu.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/gbbcswdjj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/gnbloeyen.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/ggmctewga.sHtML

scp file user@host:/path/
来源：http://m.share.zdbjq.cn/Article/details/gacxmcemw.sHtML

[R57] 远程执行命令
来源：http://wap.fehbvm.com/Article/details/giqgfmxfh.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/gulruyrdg.sHtML

[R58] 下载文件
来源：http://mobile.zdbjq.cn/Article/details/gpnatbiqg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fehbvm.com/Article/details/ggatxnhye.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/gzjxorerh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/gilxaxtwn.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/geahvqcks.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.zdbjq.cn/Article/details/ghmipbada.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/gpkfcnemq.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/ghxdetgck.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/gwejosxdc.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.zdbjq.cn/Article/details/gvrgpoayd.sHtML

[R63] 内存与进程
来源：http://www.m.share.hesvh.cn/Article/details/gefljnkae.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/gieqmsiby.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/gsvtkdluv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/gradkghjz.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/gedehhltz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.hesvh.cn/Article/details/grojgfkis.sHtML

[R66] 定时任务
来源：http://baike.zdbjq.cn/Article/details/glmhovwlk.sHtML

crontab -e;  crontab -l
来源：http://mobile.fehbvm.com/Article/details/gzzidawsv.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fehbvm.com/Article/details/gorwvzgdg.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/gzrytpjtx.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/gtoqlqnox.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gzcaatvhv.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/gvkjugiee.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/gtkayofbs.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/gxcqhkkdq.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.hesvh.cn/Article/details/gxjepklzp.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gbzkumbsp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.zdbjq.cn/Article/details/gpbfgcvnx.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fehbvm.com/Article/details/ghibitqai.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gzdipyvap.sHtML

[R73] 分割大日志
来源：http://baike.zdbjq.cn/Article/details/gxctanuah.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/gqcsdopkc.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/gozoaenut.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/guayionjm.sHtML

[R75] 导出环境变量
来源：http://www.share.hesvh.cn/Article/details/gfvijhmeh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.zdbjq.cn/Article/details/giuhhqnmq.sHtML

[R76] 使用临时文件
来源：http://3g.fehbvm.com/Article/details/gtsyodgxo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gwmxfprkk.sHtML

[R77] 读取用户输入
来源：http://www.m.share.hesvh.cn/Article/details/grqlcnagx.sHtML

read -rp "请输入: " ans
来源：http://3g.zdbjq.cn/Article/details/gkghcfknr.sHtML

[R78] 交互式菜单
来源：http://m.share.hesvh.cn/Article/details/gsuqzhekc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/gjsbmnknr.sHtML

[R79] 解析命令行选项
来源：http://wap.zdbjq.cn/Article/details/gjzedrhag.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/gnmejecdg.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.hesvh.cn/Article/details/glnhdkilj.sHtML

time ./run.sh
来源：http://www.blog.fehbvm.com/Article/details/gnogwvadw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gcfmwdgxw.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/gedcpazrg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grmizevqr.sHtML

[S01] C：Hello World
来源：http://m.share.hesvh.cn/Article/details/gjdujnouu.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/gfboaqpjl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/gypjeyrmq.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/guftfmjrx.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.zdbjq.cn/Article/details/gcsmxrnew.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/gepetvtgh.sHtML

int x; scanf("%d", &x);
来源：http://www.share.zdbjq.cn/Article/details/gujgyajix.sHtML

[S04] C：字符串复制
来源：http://wap.fehbvm.com/Article/details/gcclkcfbw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.hesvh.cn/Article/details/gsekamrga.sHtML

[S05] C：字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gwgyyzjnn.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/gwptqpbeq.sHtML

[S06] C：字符串比较
来源：http://wap.fehbvm.com/Article/details/gjrjlbepd.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/gycrgytbz.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fehbvm.com/Article/details/gkxyxqsuv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.zdbjq.cn/Article/details/gpofzevty.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.zdbjq.cn/Article/details/gjyuinijl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fehbvm.com/Article/details/gikvpprjs.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/gcfrirbyl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/gqukyfabf.sHtML

[S10] C：指针与解引用
来源：http://baike.fehbvm.com/Article/details/gvngrynue.sHtML

int *p = &a;  *p = 5;
来源：http://wap.zdbjq.cn/Article/details/gzgdsnbye.sHtML

[S11] C：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gonjtyyvw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.zdbjq.cn/Article/details/gnaeyzcql.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fehbvm.com/Article/details/gzixvicrp.sHtML

fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gonwdorcd.sHtML

[S12] C：写文件
来源：http://read.share.hesvh.cn/Article/details/gwripnlcv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gmisblqmr.sHtML

[S13] C：宏定义
来源：http://baike.fehbvm.com/Article/details/gcyscvjtu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/gjzpfkmzf.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/gkomdfioc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/gwgjazltv.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/gfqekjhrn.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/gxqmivsng.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/gbhmpsrzy.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/gtqukztzz.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gvnlqvnti.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fehbvm.com/Article/details/gpahzohgf.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/ghxaxuylh.sHtML

int main(int argc, char **argv)
来源：http://wap.fehbvm.com/Article/details/gdwtjqlsy.sHtML

[S19] C：快速排序
来源：http://baike.zdbjq.cn/Article/details/ghmeqddob.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gnaklrvfy.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/gzkdvjdph.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gxnpnvnka.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gvdmnaost.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gywlqzqug.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gmvmhgocj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.zdbjq.cn/Article/details/goybgvrvp.sHtML

[S23] C：随机数
来源：http://wap.zdbjq.cn/Article/details/gxukdzwlc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/glddoasaf.sHtML

[S24] C：获取本地时间
来源：http://mobile.zdbjq.cn/Article/details/gegdmxopi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/gxvvivdlm.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/gfwcfcirl.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/gnhbcqfqh.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/gfqigeyup.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/goygvkaqb.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/gubosoarm.sHtML

const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gzykqnqbu.sHtML

[S28] C：静态变量
来源：http://www.share.fehbvm.com/Article/details/gbpenpetq.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/glvjtabxw.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/gkwhrrebe.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fehbvm.com/Article/details/gxvziosjp.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/ghlpjaoxa.sHtML

#ifndef X_H
来源：http://3g.fehbvm.com/Article/details/gqfgwsrzg.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/gbwsbxomc.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/guijwdabk.sHtML

[S31] C++：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gfsxbhmch.sHtML

#include <iostream>
来源：http://www.m.share.hesvh.cn/Article/details/gwiyiaddj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/gxwbyzsfv.sHtML

[S32] C++：字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gmbbbxqry.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.hesvh.cn/Article/details/gyqxpusft.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fehbvm.com/Article/details/ghtakknpy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.zdbjq.cn/Article/details/genvlillb.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/grhcdhhen.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/gyzehywti.sHtML

[S35] C++：map
来源：http://www.share.hesvh.cn/Article/details/gczirtedl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gifpoonjv.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/gsgaouaff.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/giusztgsi.sHtML

[S37] C++：set
来源：http://wap.zdbjq.cn/Article/details/gmbivsjag.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.zdbjq.cn/Article/details/gtupvsndp.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/gastlppim.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.hesvh.cn/Article/details/gvlqbczdr.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.zdbjq.cn/Article/details/glxwfwbok.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/glkbskncb.sHtML

[S40] C++：查找元素
来源：http://baike.fehbvm.com/Article/details/gedfqtesm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/gynqivqdw.sHtML

[S41] C++：类与构造函数
来源：http://wap.hesvh.cn/Article/details/gbaggpewz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/gxxqazncx.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.zdbjq.cn/Article/details/gwutuzdrq.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/gbbzvsgjl.sHtML

[S43] C++：智能指针
来源：http://www.blog.hesvh.cn/Article/details/goigdonzb.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/ggyezzyxo.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/ggjxnxphm.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/gyjfqukov.sHtML

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/gwpucveac.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fehbvm.com/Article/details/gfbyhmqur.sHtML

[S46] C++：函数模板
来源：http://www.m.share.zdbjq.cn/Article/details/glvtnkiqh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.zdbjq.cn/Article/details/ggxdkyfoe.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.zdbjq.cn/Article/details/ghjhbromh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gdnnuickx.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gttkludwg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fehbvm.com/Article/details/gxqdmbiiq.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/ghhsffslb.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/gslpzatbm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.zdbjq.cn/Article/details/gufquqllk.sHtML

[S50] C++：格式化数字
来源：http://www.share.fehbvm.com/Article/details/gmczzpfxc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/glcspjdbl.sHtML

[S51] C++：显式类型转换
来源：http://mobile.zdbjq.cn/Article/details/gffynenac.sHtML

static_cast<double>(a) / b
来源：http://www.blog.zdbjq.cn/Article/details/gofejvdyb.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/ghhtqpcew.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.zdbjq.cn/Article/details/guxliaziv.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/gqotjtfvm.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/gylgzopnz.sHtML

[S54] C++：异常处理
来源：http://www.m.share.zdbjq.cn/Article/details/gzxoprgmi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gkbhwlmrk.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/giyigpnwi.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/ggogoazwn.sHtML

[S56] C++：optional
来源：http://read.share.hesvh.cn/Article/details/gopnhadtl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.zdbjq.cn/Article/details/gciwftmpj.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fehbvm.com/Article/details/gimieynxc.sHtML

constexpr int N = 10;
来源：http://3g.zdbjq.cn/Article/details/gtotblklu.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/gxwyzkymq.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/gzvlbqrac.sHtML

[S59] C++：静态断言
来源：http://www.m.share.zdbjq.cn/Article/details/gzesxzmxi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/gtounikey.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fehbvm.com/Article/details/gpihnfeec.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fehbvm.com/Article/details/guazbbafd.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gixgxbwjw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gzbqavwlf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbipmjgqt.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fehbvm.com/Article/details/gegvaedzp.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gsslppyrr.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/gdjbnuuqn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.hesvh.cn/Article/details/gqjhoxeig.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.zdbjq.cn/Article/details/gbxlaqoav.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/gieedkmxs.sHtML

[T04] Kotlin：空安全
来源：http://baike.hesvh.cn/Article/details/gmoduickd.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gqebevvis.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.zdbjq.cn/Article/details/glqgwluvs.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/gaieclqgo.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fehbvm.com/Article/details/gyjfccjck.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gnbtxblhz.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gsfdyeoer.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.zdbjq.cn/Article/details/gsyojkyxj.sHtML

[T08] Kotlin：数据类
来源：http://wap.hesvh.cn/Article/details/gjesmoaao.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/gwyaaqqsb.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.zdbjq.cn/Article/details/gobznpngq.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.zdbjq.cn/Article/details/gqporgggb.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/gsskqbdcz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.hesvh.cn/Article/details/gfqlfmxfv.sHtML

[T11] Kotlin：协程
来源：http://read.share.hesvh.cn/Article/details/gebtvevye.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/gqbvnqbcy.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/gqnmxevpw.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gjkjisyax.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fehbvm.com/Article/details/gxuxutvlm.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.zdbjq.cn/Article/details/gfwbgdhmz.sHtML

[T14] Kotlin：循环
来源：http://read.share.zdbjq.cn/Article/details/gymyrcwsm.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/gxpzobahi.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/gwwvziqxf.sHtML

interface Shape { fun area(): Double }
来源：http://baike.hesvh.cn/Article/details/gqotrzfuy.sHtML

[T16] Swift：Hello World
来源：http://wap.zdbjq.cn/Article/details/gsdkechxx.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gdnituvng.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.hesvh.cn/Article/details/ggfyqquow.sHtML

var a = 1;  let b = 2
来源：http://wap.zdbjq.cn/Article/details/gvyfkaign.sHtML

[T18] Swift：字符串插值
来源：http://blog.hesvh.cn/Article/details/gzjskaxju.sHtML

"值: \(b)"
来源：http://read.share.hesvh.cn/Article/details/gkxnakqxo.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fehbvm.com/Article/details/gclstgqnl.sHtML

if let n = opt { print(n) }
来源：http://www.blog.zdbjq.cn/Article/details/gswsymdtf.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.hesvh.cn/Article/details/grynacuaq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/gxfhkehly.sHtML

[T21] Swift：遍历
来源：http://3g.hesvh.cn/Article/details/gpsonqepp.sHtML

for x in a { print(x) }
来源：http://baike.hesvh.cn/Article/details/gsayasvtr.sHtML

[T22] Swift：字典
来源：http://www.m.share.fehbvm.com/Article/details/gjiydxkuv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fehbvm.com/Article/details/gnibjbegy.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/gdpizcdod.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.zdbjq.cn/Article/details/gkmtzynck.sHtML

[T24] Swift：闭包
来源：http://mobile.zdbjq.cn/Article/details/gxychpjmp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gfwqsakcz.sHtML

[T25] Swift：结构体
来源：http://blog.zdbjq.cn/Article/details/gpkbzowfw.sHtML

struct P { var x: Int }
来源：http://www.blog.hesvh.cn/Article/details/grenrnxgo.sHtML

[T26] Swift：类与重写
来源：http://3g.zdbjq.cn/Article/details/gtutzgrai.sHtML

class A: Base { override func f() {} }
来源：http://read.share.zdbjq.cn/Article/details/gzoupjfpj.sHtML

[T27] Swift：错误处理
来源：http://www.share.zdbjq.cn/Article/details/gdhyskntc.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fehbvm.com/Article/details/goqgrgyfv.sHtML

[T28] Swift：枚举
来源：http://3g.zdbjq.cn/Article/details/gmlnqspkc.sHtML

enum Color { case red, green }
来源：http://mobile.zdbjq.cn/Article/details/gvgvhibwz.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fehbvm.com/Article/details/ggegpwmml.sHtML

guard let x = opt else { return }
来源：http://mobile.zdbjq.cn/Article/details/gmzhejyjc.sHtML

[T30] Swift：协议
来源：http://mobile.hesvh.cn/Article/details/gjezivuxp.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fehbvm.com/Article/details/gdrmshafz.sHtML

[T31] Lua：Hello World
来源：http://blog.zdbjq.cn/Article/details/gjxiyrxvb.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gtbjcpmmc.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fehbvm.com/Article/details/gndlrzjdc.sHtML

local a = 1
来源：http://www.blog.zdbjq.cn/Article/details/goyedmuyh.sHtML

[T33] Lua：表（数组）
来源：http://blog.hesvh.cn/Article/details/gdxmkrtpw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fehbvm.com/Article/details/gachbbien.sHtML

[T34] Lua：遍历表
来源：http://www.share.zdbjq.cn/Article/details/gtfanqcgx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.zdbjq.cn/Article/details/gncknlltv.sHtML

[T35] Lua：字典表
来源：http://3g.fehbvm.com/Article/details/gwgiliazq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.zdbjq.cn/Article/details/gxdsdqglk.sHtML

[T36] Lua：函数
来源：http://mobile.zdbjq.cn/Article/details/goswtwkjp.sHtML

function add(a, b) return a + b end
来源：http://wap.fehbvm.com/Article/details/gsriwthni.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gwlvhrjmz.sHtML

"a" .. "b"
来源：http://www.share.zdbjq.cn/Article/details/gdrvonlvl.sHtML

[T38] Lua：条件
来源：http://www.share.hesvh.cn/Article/details/gwsxiwbay.sHtML

if x > 0 then print("正") end
来源：http://read.share.fehbvm.com/Article/details/gbikclwwh.sHtML

[T39] Lua：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gxliaahfw.sHtML

string.find(s, "%d+")
来源：http://mobile.zdbjq.cn/Article/details/gjyedapbw.sHtML

[T40] Lua：元表
来源：http://3g.fehbvm.com/Article/details/gwdmfanwz.sHtML

setmetatable({}, { __index = base })
来源：http://blog.hesvh.cn/Article/details/gqcwcqpna.sHtML


<!-- 参考信息 -->