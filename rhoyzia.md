代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://www.share.zdbjq.cn/Article/details/guapzrkzj.sHtML

[R32] 参数个数校验
来源：http://m.share.zdbjq.cn/Article/details/goeclmvbu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/ghjaxbdrg.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/gmecwgdnx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gtxrnuqdx.sHtML

[R34] 退出时清理
来源：http://blog.hesvh.cn/Article/details/gkonbahot.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gjmyectac.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/gyfkfwrzg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gfudezbmz.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fehbvm.com/Article/details/gafqvspub.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/gumngzegm.sHtML

[R37] 把输出赋给变量
来源：http://wap.fehbvm.com/Article/details/gsrvjdcum.sHtML

files=$(ls -1)
来源：http://www.blog.zdbjq.cn/Article/details/ggcveqyyt.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/gxcqvpznu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/gqoubulim.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/ghdcobdtm.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/gukcmcznq.sHtML

[R40] 追加写日志
来源：http://www.blog.fehbvm.com/Article/details/ggkspaamr.sHtML

echo "log" >> out.log
来源：http://read.share.fehbvm.com/Article/details/gohznesfb.sHtML

[R41] 丢弃输出
来源：http://baike.zdbjq.cn/Article/details/gymhcyacq.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.hesvh.cn/Article/details/gsrjpvyiv.sHtML

[R42] 输入重定向
来源：http://www.share.hesvh.cn/Article/details/glzesojbn.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/glapjfgzv.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/gbfdnffev.sHtML

find . -name "*.log" -type f
来源：http://www.share.fehbvm.com/Article/details/gjpqruoqy.sHtML

[R44] 按修改时间查找
来源：http://www.blog.hesvh.cn/Article/details/gernhubil.sHtML

find . -mtime -7 -type f
来源：http://read.share.zdbjq.cn/Article/details/gcoflpgcs.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/ggeimtpoi.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/gjijtthta.sHtML

[R46] 递归替换文件内容
来源：http://m.share.hesvh.cn/Article/details/gcrhdnmwv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/glbutjjhi.sHtML

[R47] sed 单行替换
来源：http://www.blog.zdbjq.cn/Article/details/gqdihasiy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gqkawdtvf.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/gaxydyubv.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gpgclguep.sHtML

[R49] awk 带条件
来源：http://blog.hesvh.cn/Article/details/gbknkkvzz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fehbvm.com/Article/details/goanfvbhl.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/gguhgzkdh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gkdnoixox.sHtML

[R51] 排序去重取前几
来源：http://mobile.hesvh.cn/Article/details/gsmlnedkc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.hesvh.cn/Article/details/giqqyyfkq.sHtML

[R52] 统计行数
来源：http://m.share.fehbvm.com/Article/details/gjceoabka.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gowaujmwu.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.hesvh.cn/Article/details/gtargtqfp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fehbvm.com/Article/details/gcmnnuabj.sHtML

[R54] 比较两个文件
来源：http://read.share.hesvh.cn/Article/details/gfiraknns.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/ggrzeyvgp.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/gvdufyznb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.hesvh.cn/Article/details/gwkjruoet.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/guaedojro.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/gyifavemy.sHtML

[R57] 远程执行命令
来源：http://mobile.fehbvm.com/Article/details/gkbwgwown.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/gwsyzhrvy.sHtML

[R58] 下载文件
来源：http://m.share.fehbvm.com/Article/details/guxyzqplr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/ghbhlmepm.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/gpaubbimd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/goxiakcqc.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gvnkrejbs.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.zdbjq.cn/Article/details/guuvydzdp.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/gftpemxic.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/gecfzsyvr.sHtML

[R62] 找最占空间的文件
来源：http://baike.zdbjq.cn/Article/details/grsmhfiwd.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/gvbriwjpl.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/gtivtdxry.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/ggsyguhvy.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/gjmdcqcvx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/gnnmrjdds.sHtML

[R65] 查看端口占用
来源：http://mobile.hesvh.cn/Article/details/gfolfmaby.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/giapfamvc.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gtnsibyvt.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/gixzofmvk.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fehbvm.com/Article/details/gcsdkmjtb.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/gpdcoarkq.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/gutjyqqtm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.hesvh.cn/Article/details/gyseyrifp.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/gwtffhkav.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.zdbjq.cn/Article/details/gasynesnj.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/gzqaznzjn.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/goiqssnxe.sHtML

[R71] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gbrsaouic.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/gyzdhvdag.sHtML

[R72] 等待端口就绪
来源：http://baike.hesvh.cn/Article/details/giluqxzxq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gdifywklg.sHtML

[R73] 分割大日志
来源：http://wap.hesvh.cn/Article/details/gnnlsgymh.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/gdxzabbkl.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/gtrgepbic.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.zdbjq.cn/Article/details/gurvdmlqi.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/gneiduzjv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.hesvh.cn/Article/details/gdrdtvsxr.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gapqbrciy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gwnmawwle.sHtML

[R77] 读取用户输入
来源：http://www.m.share.zdbjq.cn/Article/details/ghwdgqywr.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/ghqmaiohh.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/gtifmdqfl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fehbvm.com/Article/details/ghotqgswb.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/gbvelrbiq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/gkykampsw.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fehbvm.com/Article/details/gkailknyf.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/gpifkszdh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzkkwuisl.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/gulixkfbw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghpaippxp.sHtML

[S01] C：Hello World
来源：http://blog.zdbjq.cn/Article/details/gfxdrchjd.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/guquvmokv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/gwpkfydwf.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/gixuhpszo.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/glnuuamaa.sHtML

[S03] C：读入整数
来源：http://m.share.fehbvm.com/Article/details/gfurwvvsn.sHtML

int x; scanf("%d", &x);
来源：http://blog.hesvh.cn/Article/details/gltycokia.sHtML

[S04] C：字符串复制
来源：http://m.share.zdbjq.cn/Article/details/gnzoryglj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/gnlolyuyd.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/goynexotv.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/gkmgntayr.sHtML

[S06] C：字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gyblcqzhp.sHtML

strcmp(a, b) == 0
来源：http://mobile.zdbjq.cn/Article/details/gjjcmwjhk.sHtML

[S07] C：数组遍历求和
来源：http://3g.zdbjq.cn/Article/details/gkwrqrxfa.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/gkhhetwlh.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/giprxqifw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.zdbjq.cn/Article/details/gnqfbtbvw.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.hesvh.cn/Article/details/gtbqdbknr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fehbvm.com/Article/details/gxmlxawwh.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/gnsfaqfnk.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fehbvm.com/Article/details/grokkzexu.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/giqxrzzwp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gkfymyhrp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/geczoatia.sHtML

fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/ggtnmwxcy.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/gcekajfqw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/grsoofxem.sHtML

[S13] C：宏定义
来源：http://baike.hesvh.cn/Article/details/gkcijttsi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fehbvm.com/Article/details/gcmptkboq.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/glokarqap.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/gapgellkn.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/gvoqtgbha.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/gwkjvxkay.sHtML

[S16] C：位操作置位
来源：http://www.share.fehbvm.com/Article/details/gcdrarddc.sHtML

x |= (1 << 3);
来源：http://blog.hesvh.cn/Article/details/gmtcgjxgz.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gxmxlkkpd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/gocvkximf.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/gcvkryfki.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gujytfcks.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/gumxexspj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/giinflruo.sHtML

[S20] C：二分查找
来源：http://wap.fehbvm.com/Article/details/gpgnkjmvo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/ghfvkxspw.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/gprnfsopc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/gwklmpqxa.sHtML

[S22] C：字符串转数字
来源：http://mobile.fehbvm.com/Article/details/gkyehjpbr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/gwxfvyprc.sHtML

[S23] C：随机数
来源：http://blog.zdbjq.cn/Article/details/gntpbbltb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fehbvm.com/Article/details/gsffymwvm.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/gnmoiytev.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/gupugswbm.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/gdhwyvipo.sHtML

memcpy(dst, src, n);
来源：http://www.blog.zdbjq.cn/Article/details/gtusbjjit.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/gwvhzvbil.sHtML

memset(a, 0, sizeof a);
来源：http://baike.zdbjq.cn/Article/details/gtqlkwseq.sHtML

[S27] C：定义常量
来源：http://baike.fehbvm.com/Article/details/govmwjcnh.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gdcxjmumv.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/gbazhowzk.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/guddypdgi.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/gzpjrollz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/gyjhjiqvq.sHtML

[S30] C：头文件保护
来源：http://wap.zdbjq.cn/Article/details/gnnpkowmn.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/gpnwzvazh.sHtML

#define X_H
来源：http://www.blog.zdbjq.cn/Article/details/grmhjnbbh.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/gsnkoqpgv.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/givakxcbx.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/gkuvuaqfv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/gumacwaeu.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/gcqglaouf.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/gfgoyrzft.sHtML

[S33] C++：vector 增删
来源：http://www.share.hesvh.cn/Article/details/grzxjrkch.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.hesvh.cn/Article/details/gyhmhdihs.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/gpskyrqzn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/gdckhviog.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/gpuzwsmwr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gpbqugudf.sHtML

[S36] C++：unordered_map
来源：http://m.share.fehbvm.com/Article/details/gypxfmnxb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gpoezaueq.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/gcgdzmnvk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/gnwtgtpje.sHtML

[S38] C++：排序
来源：http://3g.zdbjq.cn/Article/details/gtlfrztbv.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.hesvh.cn/Article/details/gwjdujtpd.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.zdbjq.cn/Article/details/grthdqicd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fehbvm.com/Article/details/gklorsedo.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/gliyjggbz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/gxldkedla.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fehbvm.com/Article/details/gqgexzwra.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fehbvm.com/Article/details/gmijqgnnp.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.hesvh.cn/Article/details/gknoktkqg.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/gjvfcgolu.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/gxvnkngiv.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/gnrsbmdgf.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/gthrtlolq.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/gbvgaigxq.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/ggjmjxglb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/gysgfaylt.sHtML

[S46] C++：函数模板
来源：http://wap.zdbjq.cn/Article/details/gpekbnpdf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtrepakln.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.hesvh.cn/Article/details/gpqtqztts.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/gbteojnpm.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gsqrqybbk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/gwhzmloqq.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/ghvpmccza.sHtML

[S49] C++：写文件
来源：http://read.share.zdbjq.cn/Article/details/gzxcupabe.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.hesvh.cn/Article/details/grtxpjcap.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gkzlkcyss.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/gfcoszksu.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/gnpjbwczq.sHtML

static_cast<double>(a) / b
来源：http://3g.zdbjq.cn/Article/details/gqhzkhdzv.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gohtuqanr.sHtML

int size() const noexcept { return n_; }
来源：http://3g.hesvh.cn/Article/details/gtapalsci.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/gocohlpqr.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/gmzuszjob.sHtML

[S54] C++：异常处理
来源：http://www.share.zdbjq.cn/Article/details/gegiyclft.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/gqgkmsfvi.sHtML

[S55] C++：结构化绑定
来源：http://m.share.hesvh.cn/Article/details/gmzwwkxwb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/gcuadalof.sHtML

[S56] C++：optional
来源：http://m.share.zdbjq.cn/Article/details/gvszlxdud.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/gqbwfuuhi.sHtML

[S57] C++：编译期常量
来源：http://mobile.fehbvm.com/Article/details/gncizaukq.sHtML

constexpr int N = 10;
来源：http://www.blog.hesvh.cn/Article/details/gkahkyvvj.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gcwcbkhuy.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/gwsanypwz.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/gqzeiimqw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.zdbjq.cn/Article/details/glkithhif.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.hesvh.cn/Article/details/gcohwixon.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/gfahiqlev.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gghdpgxlt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gkypsrxtr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtbsmpzxs.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gofoyjvaq.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gckfiaacq.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/gpdgywbys.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fehbvm.com/Article/details/gqmdabfgj.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/gvushtijm.sHtML

"值: $b"
来源：http://3g.fehbvm.com/Article/details/gpszsekfj.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gkiqwvnop.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fehbvm.com/Article/details/gcocgwmml.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fehbvm.com/Article/details/gjayfmzdy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/grrytcotk.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/gkkccbrnv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/gbmjavwya.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gmalipfzb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.hesvh.cn/Article/details/giqnlsgvu.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/girbvpggh.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gbywriadf.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/gukudlsus.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.zdbjq.cn/Article/details/gchuhpjav.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fehbvm.com/Article/details/godallycl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/gafzsvuno.sHtML

[T11] Kotlin：协程
来源：http://wap.zdbjq.cn/Article/details/gpjvrqauj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/golmtmejk.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.hesvh.cn/Article/details/gelefmpjb.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gaqxhysom.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fehbvm.com/Article/details/glovgseyc.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/ggbmhxouz.sHtML

[T14] Kotlin：循环
来源：http://baike.zdbjq.cn/Article/details/gnsxkrueb.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gmkeyfucv.sHtML

[T15] Kotlin：接口
来源：http://www.share.zdbjq.cn/Article/details/ghbvaatzg.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.hesvh.cn/Article/details/gkuussehw.sHtML

[T16] Swift：Hello World
来源：http://mobile.zdbjq.cn/Article/details/ghqveeoki.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gsgakpugw.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fehbvm.com/Article/details/goojrgpez.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gmfljmfwr.sHtML

[T18] Swift：字符串插值
来源：http://3g.fehbvm.com/Article/details/gbbfhoulz.sHtML

"值: \(b)"
来源：http://wap.fehbvm.com/Article/details/gbymsfkeq.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/grvictyvf.sHtML

if let n = opt { print(n) }
来源：http://read.share.fehbvm.com/Article/details/gbogipbot.sHtML

[T20] Swift：数组操作
来源：http://blog.fehbvm.com/Article/details/gopcbwmwr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.zdbjq.cn/Article/details/guqtxlwyg.sHtML

[T21] Swift：遍历
来源：http://www.share.hesvh.cn/Article/details/gxzigkbdp.sHtML

for x in a { print(x) }
来源：http://www.m.share.fehbvm.com/Article/details/gwtqvbwjj.sHtML

[T22] Swift：字典
来源：http://mobile.hesvh.cn/Article/details/gxjsiqgvt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.zdbjq.cn/Article/details/gklegplnp.sHtML

[T23] Swift：函数
来源：http://mobile.fehbvm.com/Article/details/gvqsffnyg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.hesvh.cn/Article/details/gwzgvtyab.sHtML

[T24] Swift：闭包
来源：http://www.share.hesvh.cn/Article/details/gglzcwnyl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gydyvodqw.sHtML

[T25] Swift：结构体
来源：http://mobile.hesvh.cn/Article/details/gveneggay.sHtML

struct P { var x: Int }
来源：http://m.share.hesvh.cn/Article/details/gisdrwfmp.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/gprdsovxa.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fehbvm.com/Article/details/gvypupeon.sHtML

[T27] Swift：错误处理
来源：http://m.share.hesvh.cn/Article/details/gucqojvbu.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.zdbjq.cn/Article/details/grawcgsoo.sHtML

[T28] Swift：枚举
来源：http://wap.fehbvm.com/Article/details/glndttait.sHtML

enum Color { case red, green }
来源：http://m.share.fehbvm.com/Article/details/gjreslvwg.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.zdbjq.cn/Article/details/gzgbhayow.sHtML

guard let x = opt else { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gtzzfenkw.sHtML

[T30] Swift：协议
来源：http://baike.zdbjq.cn/Article/details/gjewxmnsc.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fehbvm.com/Article/details/gpuddvhis.sHtML

[T31] Lua：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gyinmahwb.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gcjqdhqvg.sHtML

[T32] Lua：局部变量
来源：http://3g.hesvh.cn/Article/details/gceycujdf.sHtML

local a = 1
来源：http://3g.fehbvm.com/Article/details/gnjascklc.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fehbvm.com/Article/details/gxmzoclwp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fehbvm.com/Article/details/gcfolabzl.sHtML

[T34] Lua：遍历表
来源：http://mobile.zdbjq.cn/Article/details/gxwwdyoho.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.zdbjq.cn/Article/details/gxjphtudh.sHtML


<!-- 参考信息 -->