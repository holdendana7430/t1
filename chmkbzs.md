代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.zdbjq.cn/Article/details/gsrplgnug.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fehbvm.com/Article/details/gdkvgyvrm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.hesvh.cn/Article/details/gzvrmeowj.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/gzizjxsty.sHtML

files=$(ls -1)
来源：http://m.share.fehbvm.com/Article/details/gtjltecer.sHtML

[R38] 管道串联
来源：http://www.blog.fehbvm.com/Article/details/gqpjinilv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fehbvm.com/Article/details/gtagadxmf.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.hesvh.cn/Article/details/gjezyeytc.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gwnjdeszz.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/gutifdzkg.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/ghksraeiz.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gijfpgqxz.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/ggspbastl.sHtML

[R42] 输入重定向
来源：http://mobile.zdbjq.cn/Article/details/gfcxzurlt.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/gxysapgxw.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/gbkzlpxyl.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/gtlboqits.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/gzbmexnje.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/gtcxswqos.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/gecluaqmv.sHtML

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/gczxjgxkz.sHtML

[R46] 递归替换文件内容
来源：http://3g.hesvh.cn/Article/details/gaodvnbvj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/ghkbcmtwu.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/gwngjdkgs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/gktoajhtb.sHtML

[R48] awk 取指定列
来源：http://www.blog.zdbjq.cn/Article/details/gebpjjkfe.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gzaaawkpo.sHtML

[R49] awk 带条件
来源：http://wap.hesvh.cn/Article/details/gygpcecwo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.zdbjq.cn/Article/details/gowkqwidg.sHtML

[R50] awk 求和
来源：http://wap.hesvh.cn/Article/details/gkclwhyac.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/ginhzcemp.sHtML

[R51] 排序去重取前几
来源：http://blog.hesvh.cn/Article/details/gnwbxeogm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/gfgucysqx.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/gukyuxpxo.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gxhthtlmp.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.zdbjq.cn/Article/details/gpwrylmsl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.hesvh.cn/Article/details/ghwcwmury.sHtML

[R54] 比较两个文件
来源：http://www.blog.fehbvm.com/Article/details/gpxditmrl.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/gyenmogdi.sHtML

[R55] 压缩与解压
来源：http://www.blog.hesvh.cn/Article/details/gybddccrj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fehbvm.com/Article/details/gqddlzfsj.sHtML

[R56] 远程拷贝
来源：http://m.share.zdbjq.cn/Article/details/gfgkfhhvc.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/gynhpyvyb.sHtML

[R57] 远程执行命令
来源：http://mobile.fehbvm.com/Article/details/gwdjwdiok.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/gogeoukhq.sHtML

[R58] 下载文件
来源：http://read.share.hesvh.cn/Article/details/giautxdue.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.hesvh.cn/Article/details/gnyzkrjyk.sHtML

[R59] 发 POST JSON
来源：http://wap.hesvh.cn/Article/details/geaeyhvzt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/grevxnxvw.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gnuaepcdj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.zdbjq.cn/Article/details/ggnjcrmcs.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/glfxqhtub.sHtML

df -h;  du -sh *
来源：http://www.blog.hesvh.cn/Article/details/gohgoamex.sHtML

[R62] 找最占空间的文件
来源：http://baike.fehbvm.com/Article/details/grcnepaaa.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/gyzpowjoz.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/gicjlsetu.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/gqwucyekw.sHtML

[R64] 结束进程
来源：http://wap.zdbjq.cn/Article/details/gmdrnbpmq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.hesvh.cn/Article/details/gtppfzwvv.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/gslduxluy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.hesvh.cn/Article/details/gfengvumt.sHtML

[R66] 定时任务
来源：http://blog.zdbjq.cn/Article/details/gwocmquag.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.hesvh.cn/Article/details/gaigeehsh.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/gzbhbesuw.sHtML

openssl rand -hex 16
来源：http://www.blog.hesvh.cn/Article/details/gwzxxklme.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/gsuyvronk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.hesvh.cn/Article/details/gmhabfwse.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fehbvm.com/Article/details/gjinmlmup.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gmxtgtmqh.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/gcevzlnox.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/gpwnzpxtw.sHtML

[R71] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gluiijvnu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/gngmfrzxj.sHtML

[R72] 等待端口就绪
来源：http://wap.hesvh.cn/Article/details/geznecnsk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gitmergkp.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/gpfwhpqdn.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/ggbnefrpl.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/gsldyporu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/gxpgirhlb.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/geltrpgga.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/gjufeavgb.sHtML

[R76] 使用临时文件
来源：http://m.share.fehbvm.com/Article/details/ghsqlxpvo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gludmlsij.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gptggumlg.sHtML

read -rp "请输入: " ans
来源：http://m.share.zdbjq.cn/Article/details/gduzajorl.sHtML

[R78] 交互式菜单
来源：http://3g.zdbjq.cn/Article/details/gsjretncl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/gjtvvdvnv.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/gshxwtmhu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fehbvm.com/Article/details/gajvmffqj.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.hesvh.cn/Article/details/gnktrpxwl.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/gkutjsdjz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmphtfzbx.sHtML

S. C / C++ 专题
来源：http://3g.hesvh.cn/Article/details/gwzqubxvr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gianfdapr.sHtML

[S01] C：Hello World
来源：http://mobile.fehbvm.com/Article/details/guzfywxdm.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/ghhvgivyb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fehbvm.com/Article/details/gnigloksh.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/ggzxpnqqx.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.zdbjq.cn/Article/details/gajzbzcyi.sHtML

[S03] C：读入整数
来源：http://m.share.fehbvm.com/Article/details/gyhvlbmgx.sHtML

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/gifjcienf.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/gmfmojedq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gglowdseq.sHtML

[S05] C：字符串长度
来源：http://blog.zdbjq.cn/Article/details/gxotgbhwr.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/gqpyeknzf.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gxfqqwmid.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/gjkmhnqqo.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/gmwanvjue.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fehbvm.com/Article/details/gtkpkapfm.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/gjrownwqj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/gwlwxqizx.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/gdayjawyt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gvalhmjmw.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/gvgdxeekx.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fehbvm.com/Article/details/gzboajxcu.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gizbpfttf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.hesvh.cn/Article/details/guscnhttq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/groidgthm.sHtML

fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/guaovrgje.sHtML

[S12] C：写文件
来源：http://www.share.fehbvm.com/Article/details/gfyprjsdg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gznjcddmc.sHtML

[S13] C：宏定义
来源：http://www.share.fehbvm.com/Article/details/gpzkcuevx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/gxgudaxus.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/ggfcxdkkr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gfececgpk.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/giylnqkaf.sHtML

(double) a / b
来源：http://3g.hesvh.cn/Article/details/gbzrdfode.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/gergefmge.sHtML

x |= (1 << 3);
来源：http://m.share.zdbjq.cn/Article/details/gjklyudpr.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gstgvofjt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.zdbjq.cn/Article/details/glnoalyyx.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/gdryqkdwx.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/gwivhcild.sHtML

[S19] C：快速排序
来源：http://m.share.hesvh.cn/Article/details/gzvztqejv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gbrsqluuz.sHtML

[S20] C：二分查找
来源：http://wap.zdbjq.cn/Article/details/gcuxqoayr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gxvcbvfxs.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/gzeqtlwdf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.hesvh.cn/Article/details/gqkjbmpzi.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/geatljvei.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.hesvh.cn/Article/details/gpblifhsr.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/guswogash.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/gywabkpbp.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/goktejhky.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.hesvh.cn/Article/details/geoxxaoqu.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/gcvbzaufw.sHtML

memcpy(dst, src, n);
来源：http://baike.hesvh.cn/Article/details/gfandqgot.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/gamyabebm.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gxfpwmljd.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/gslahiibs.sHtML

const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/ghamyfejd.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/glutnzcsl.sHtML

static int counter = 0;
来源：http://3g.zdbjq.cn/Article/details/gjnunruxk.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/geiddzkne.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fehbvm.com/Article/details/gjlbwoliu.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/gukyauflj.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/ghhqhqjje.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/goshmrywn.sHtML

#endif
来源：http://www.m.share.fehbvm.com/Article/details/gcosfewwx.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gkplousla.sHtML

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/gahkxvzog.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/ggppqugci.sHtML

[S32] C++：字符串
来源：http://www.m.share.hesvh.cn/Article/details/gqgceyujg.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gqjzvcjxh.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/gjqmzatyt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gwefkyycv.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/gtddoqnhr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fehbvm.com/Article/details/gawiieuxa.sHtML

[S35] C++：map
来源：http://www.blog.hesvh.cn/Article/details/gmoebrazz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gpvhopsjs.sHtML

[S36] C++：unordered_map
来源：http://3g.zdbjq.cn/Article/details/gkzyaowme.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gybivwcac.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/gvgjtdhmx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.zdbjq.cn/Article/details/gkdwcomwo.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/gzodjpdqm.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gukkndpbd.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fehbvm.com/Article/details/grtleswph.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/geememmvn.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/gionoropi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fehbvm.com/Article/details/gtxjcrrlf.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/gywfohwen.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/ggobefpva.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/glmlgbljr.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.hesvh.cn/Article/details/groylyizc.sHtML

[S43] C++：智能指针
来源：http://baike.fehbvm.com/Article/details/gxarhkesw.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/gjucwauxy.sHtML

[S44] C++：引用传参
来源：http://wap.fehbvm.com/Article/details/gqzmstxwz.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/gdeurqinx.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/ggndbpquh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/ghnroovnr.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/gknkwwwvk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.zdbjq.cn/Article/details/gnnerzggk.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/gbmbspmuu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/gyjogdore.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gxudmqlxx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/ggmydsghn.sHtML

while (std::getline(in, line)) { }
来源：http://baike.zdbjq.cn/Article/details/gbslhhmon.sHtML

[S49] C++：写文件
来源：http://blog.zdbjq.cn/Article/details/gfgbobezu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.zdbjq.cn/Article/details/gwaizfulu.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gbyzkymab.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gsnktuxul.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fehbvm.com/Article/details/ghzcghvfn.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/guchwfrcg.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/gcfmvgylh.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/gfbkaheis.sHtML

[S53] C++：移动语义
来源：http://mobile.zdbjq.cn/Article/details/gjtfpwsrr.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fehbvm.com/Article/details/giukekqfw.sHtML

[S54] C++：异常处理
来源：http://www.share.zdbjq.cn/Article/details/gmrvlqdif.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/gftgkyinl.sHtML

[S55] C++：结构化绑定
来源：http://wap.zdbjq.cn/Article/details/gzmbtpbbj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gpvygnikl.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gyvgsfuti.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.zdbjq.cn/Article/details/gnhkvkcyv.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/gxxzejosi.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/gxaacplpi.sHtML

[S58] C++：命名空间
来源：http://wap.fehbvm.com/Article/details/gyxkmliea.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/gykxyoxeh.sHtML

[S59] C++：静态断言
来源：http://read.share.fehbvm.com/Article/details/gncqpezmo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.zdbjq.cn/Article/details/gqtjkxgwx.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.hesvh.cn/Article/details/gkzlsgrwk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fehbvm.com/Article/details/gazauyrnf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gozkfbqfz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/grjioygzy.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glwcqfnrn.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gwkiimdno.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/grpyrzmjg.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/ghpmwvsxo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fehbvm.com/Article/details/govdbxxod.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/gbexnbvoz.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/gchyisxjd.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gnvbrasbc.sHtML

val n: String? = null;  n?.length
来源：http://baike.fehbvm.com/Article/details/gwwhwuhwb.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fehbvm.com/Article/details/gzabafvtr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.zdbjq.cn/Article/details/gshysbpud.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gmjyxtyxk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.zdbjq.cn/Article/details/gsyxxypof.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gnymxdkjq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.zdbjq.cn/Article/details/gwvogofxl.sHtML

[T08] Kotlin：数据类
来源：http://baike.fehbvm.com/Article/details/gqhcdliia.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/gcmscwvbu.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.hesvh.cn/Article/details/gpclfrtyf.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gfcuajpqc.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.hesvh.cn/Article/details/godzifkws.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.zdbjq.cn/Article/details/gdroafizc.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/gldyzuysn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.hesvh.cn/Article/details/gtbldabhc.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/grlswrome.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gpyefnayd.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/gehnarbeb.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.hesvh.cn/Article/details/grspdfsct.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gvynsnpgt.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/ggnolqtpf.sHtML

[T15] Kotlin：接口
来源：http://m.share.hesvh.cn/Article/details/gdihhwvnn.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.zdbjq.cn/Article/details/gkmmlfdxr.sHtML

[T16] Swift：Hello World
来源：http://baike.zdbjq.cn/Article/details/gcjuuiqaj.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/ghvztjgve.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/gemynavts.sHtML

var a = 1;  let b = 2
来源：http://www.blog.hesvh.cn/Article/details/ggvkzjvll.sHtML

[T18] Swift：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gygsqlyti.sHtML

"值: \(b)"
来源：http://www.blog.hesvh.cn/Article/details/gqfurwjwr.sHtML

[T19] Swift：可选绑定
来源：http://m.share.hesvh.cn/Article/details/gxbfghstc.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/gcopsscar.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.zdbjq.cn/Article/details/grsxtovhc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fehbvm.com/Article/details/ggbyulere.sHtML

[T21] Swift：遍历
来源：http://www.share.hesvh.cn/Article/details/gjgenamsu.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/gltxbbydf.sHtML

[T22] Swift：字典
来源：http://www.m.share.hesvh.cn/Article/details/gpmnkxonq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.hesvh.cn/Article/details/gfleubnka.sHtML

[T23] Swift：函数
来源：http://wap.zdbjq.cn/Article/details/gtumlmtkw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.hesvh.cn/Article/details/glywvdpsd.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/gsbwvzbfv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/ghyodghlh.sHtML

[T25] Swift：结构体
来源：http://mobile.hesvh.cn/Article/details/gikwqahdw.sHtML

struct P { var x: Int }
来源：http://www.share.hesvh.cn/Article/details/gfwvfgwvj.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/gmalgdwqu.sHtML

class A: Base { override func f() {} }
来源：http://blog.fehbvm.com/Article/details/gikamqavr.sHtML

[T27] Swift：错误处理
来源：http://www.share.zdbjq.cn/Article/details/gcvetpaes.sHtML

do { try f() } catch { print(error) }
来源：http://baike.hesvh.cn/Article/details/gfjeedbnv.sHtML

[T28] Swift：枚举
来源：http://blog.fehbvm.com/Article/details/gojcvnfdg.sHtML

enum Color { case red, green }
来源：http://read.share.hesvh.cn/Article/details/ghzuisoqa.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.zdbjq.cn/Article/details/gpneddnmu.sHtML

guard let x = opt else { return }
来源：http://wap.hesvh.cn/Article/details/gdrcmngdq.sHtML

[T30] Swift：协议
来源：http://mobile.hesvh.cn/Article/details/giiporfzj.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fehbvm.com/Article/details/gxrrkkpcs.sHtML

[T31] Lua：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gvydhdsxm.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gsbewgpst.sHtML

[T32] Lua：局部变量
来源：http://3g.fehbvm.com/Article/details/ghkjgqfiz.sHtML

local a = 1
来源：http://blog.hesvh.cn/Article/details/gmwerltcn.sHtML

[T33] Lua：表（数组）
来源：http://read.share.zdbjq.cn/Article/details/gizouezcs.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fehbvm.com/Article/details/gewmlbaip.sHtML

[T34] Lua：遍历表
来源：http://blog.fehbvm.com/Article/details/gyczawvay.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/gwpfawwod.sHtML

[T35] Lua：字典表
来源：http://wap.zdbjq.cn/Article/details/gehkdymlu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fehbvm.com/Article/details/gfacuegxd.sHtML

[T36] Lua：函数
来源：http://blog.zdbjq.cn/Article/details/geravropg.sHtML

function add(a, b) return a + b end
来源：http://www.blog.hesvh.cn/Article/details/gjkzmufbb.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/gaslsaebl.sHtML

"a" .. "b"
来源：http://3g.zdbjq.cn/Article/details/gsnqxglma.sHtML

[T38] Lua：条件
来源：http://mobile.fehbvm.com/Article/details/gzmmwvcqe.sHtML

if x > 0 then print("正") end
来源：http://wap.hesvh.cn/Article/details/gkrzideks.sHtML


<!-- 参考信息 -->