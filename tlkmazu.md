代发 wailian999

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/grnztheyh.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamxfppnj.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvfydguq.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbdtdigj.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gntqtnybm.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gpmxivbah.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gubxuvnqu.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gngcruknp.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/gzualfmua.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzwocayy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnsnqmej.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmmpuufa.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/guydnwshi.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnaiwapc.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gzfoserpi.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gtslippsp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/ghhkqrzgl.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gnclwqvfj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqswmelb.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqhisffj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/guxqogbwf.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gkqltddsg.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsyckkbhd.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gcetfzuiv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/giedsyznk.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjbvbsxh.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/galtdyimd.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/glwjmmhar.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlokmwtf.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfmsoqpk.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/gaojuuzvi.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gqmkcudan.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxjusuyw.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gmublswyc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjefodum.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gnuofdygm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/grbrbukip.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmkelmtt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/gxuyrrqgv.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gcnsgsfih.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gdiomohdo.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlzmuips.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/ggwdvqspb.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrzaqqxz.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gngyigokr.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxhckztw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/geptgzgzx.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/gxllnpxen.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gjfmqpiyd.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfipgtcy.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gnmsypzsp.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gopjjvkli.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gjiaiqetm.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gdovnqmvp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gdqulpimo.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbtqyymm.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gwmqhkwvi.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gsdkphpln.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gegeiprae.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbklwowts.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/geyknzgbr.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllrxhbtu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gppenohkw.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gxncyelih.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gtoojefqg.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gbhtktwlb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyyuwhsy.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gjafitirb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfvgafkt.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/grphkoxqh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gwytamemq.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtgsucyo.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gsletdijw.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvmylyqd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/grkgpksvn.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gxaplhdqd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzjttleb.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkzzpezw.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gltfaeofh.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gbkppeajq.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/giptcvllm.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwoqvlklt.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gnahpptke.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdjrwdcf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzyenfopo.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gtdejesko.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gxqmhbrhp.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gshrquids.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gnvrxnqmk.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/geeojyhux.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gclsgwkii.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gttrqchou.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqrekasb.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/googayrlz.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/goqdjaicc.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/glwnumevl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhxxsgxs.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhytypvd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhpfklre.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzyaooewx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gfimkmqvs.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gdknhqsly.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjyflpqx.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/guwqidxvk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gkuuyvzzx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcefaeea.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/goedeyklh.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gguzwzrry.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gmfevcadn.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/gpokxdmid.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzfsalol.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gutajoddx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhkbyufe.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gcudfiwse.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofteeuse.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbhbyjmg.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gvybdbyrk.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufaiidky.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqturekgg.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gsieactep.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gfdnrvywq.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gsvrkmzxe.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/glrbhybou.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gacaogcdl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpyejsng.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/goppfnnyt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjxqcsgs.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gefzwahkg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/ggazbsbhy.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/grjjedhad.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxydlzbe.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/grokmcboi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gudxwpojf.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gjeeudmud.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goypshpyo.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gwxwyoilj.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gtonlbdke.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gtzscnegi.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpnxvmhu.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/guwplcxcs.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guskpejir.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqbhwpxf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/guejlgfvf.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtftcpgj.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gijmrhmmv.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzjzcgdf.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/gnugmfwqe.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewcnqipb.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvhurahh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gquxvqhpr.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gcwtcdogp.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlmqweng.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gdrcpiclr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgqieftj.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/gipwddgms.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzsyjjyqi.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdkqhyvy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcplgfqoc.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrhdupbx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdsdtlir.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/godteasci.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gddtpyjvh.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtyedsnre.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gwajuxjdm.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkltzilq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gkiaaofrb.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gfuxlcgfg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxykojmj.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqfyotzt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gtuptuaki.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/gmdininjk.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlwsjjua.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/geschglyt.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqmhegpu.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gdlufjbuj.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gessapsnw.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvdqzkas.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdgbltzj.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gjadkojar.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzppgese.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpxjfjzz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqpfabdn.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbypblbpy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcfewcbm.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/giteicrof.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gwexaboqw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/guujxhwvf.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzoivguv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gjzhcgsuq.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/glipvcbzh.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/gclgztpds.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/gcmuywjen.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/gkzrgtubx.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/gdakglbdz.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/geicmvzwo.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gejpcbkhv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxuwitdf.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgklbvdv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gayzvtqsy.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goywbsoyo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkhdnukmm.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxlyuwqr.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmgoxwfy.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gqxyuounp.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gjijvcsmn.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsthogpd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/ggeqymzuk.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gyffrkdti.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gngborblm.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gxqsuuhoj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/gbftisxsm.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gptiyubhn.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxoeuprn.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/geycetpok.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gqauxriok.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gstjshwyk.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fanxiaobao.xyz/Article/details/gjjhojzrr.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvlgdefm.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnmftowo.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/guntxebym.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvtskvws.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fanxiaobao.xyz/Article/details/gfuuvdfuj.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gnravznhi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gybljczdx.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gycwducki.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/gnwaqghcq.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/ghflhrzyu.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfptfnegr.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/gjhzcjdcm.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gslcboefb.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/ggokfdlpt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/gykygkdlp.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/gruhvqqex.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/gftbqnngd.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gioonljmu.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxuahblrp.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxmystsm.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhwlsiza.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gyjrfsohj.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvybkfjlm.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdrccuvy.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gmikuimpi.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gcuhqixqx.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gldggvran.sHtML

[T17] Swift：变量与常量
来源：http://baike.fanxiaobao.xyz/Article/details/gkxgmqmgq.sHtML

var a = 1;  let b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnpteuwm.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsifvvsk.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/gpfxjnylz.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gioookxnt.sHtML

if let n = opt { print(n) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gewpbimwc.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/gaqqjsuql.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvyklyev.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/ggmhpvduh.sHtML

for x in a { print(x) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxmulchf.sHtML

[T22] Swift：字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwsqmaev.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gtnbufsfh.sHtML

[T23] Swift：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gqoyxfjan.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/gjbzizdfo.sHtML

[T24] Swift：闭包
来源：http://3g.fanxiaobao.xyz/Article/details/gdnzjwcgm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfhfcqfh.sHtML

[T25] Swift：结构体
来源：http://www.blog.fanxiaobao.xyz/Article/details/grctcnggs.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshawlomz.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guuakvjhv.sHtML

class A: Base { override func f() {} }
来源：http://3g.fanxiaobao.xyz/Article/details/gdtotndxt.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghunnqvee.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxcklbta.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/glmpxqyju.sHtML

enum Color { case red, green }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzumgxqrb.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/gwzdrzrct.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxzjxdrx.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/gpilqucxq.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gckcpqprh.sHtML

[T31] Lua：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpepnwmp.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gnfulvppu.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltlqbcni.sHtML

local a = 1
来源：http://3g.fanxiaobao.xyz/Article/details/gxscvmjnm.sHtML

[T33] Lua：表（数组）
来源：http://baike.fanxiaobao.xyz/Article/details/gfggnjdwu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fanxiaobao.xyz/Article/details/gedhppphf.sHtML

[T34] Lua：遍历表
来源：http://m.share.fanxiaobao.xyz/Article/details/goqmplbxd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fanxiaobao.xyz/Article/details/gmiefumqr.sHtML

[T35] Lua：字典表
来源：http://m.share.fanxiaobao.xyz/Article/details/gssreqydf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gdokdxjpg.sHtML

[T36] Lua：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gqtvconce.sHtML

function add(a, b) return a + b end
来源：http://read.share.fanxiaobao.xyz/Article/details/gisxrrglk.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpzunzos.sHtML

"a" .. "b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwzemsye.sHtML

[T38] Lua：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhsmfkce.sHtML

if x > 0 then print("正") end
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmomrllq.sHtML

[T39] Lua：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gxjjrmjkr.sHtML

string.find(s, "%d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gwygiivdc.sHtML

[T40] Lua：元表
来源：http://blog.fanxiaobao.xyz/Article/details/gxlqptvkr.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/glvcinkld.sHtML

[T41] Perl：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/garnzvbei.sHtML

print "Hello\n";
来源：http://3g.fanxiaobao.xyz/Article/details/goncjpyoh.sHtML

[T42] Perl：变量类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gxluvueau.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmgoeokl.sHtML

[T43] Perl：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gjrvyvauo.sHtML

"值: $a"
来源：http://3g.fanxiaobao.xyz/Article/details/glgeusper.sHtML

[T44] Perl：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gpwstjxwv.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gixdxvkxe.sHtML


<!-- 参考信息 -->