代发 wailian999

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxyrpdue.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/grwlubxmf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqdwtgmc.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gquzyyzor.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gcbchhkiv.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gfhodntdb.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjcwkned.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gjrhzvwjp.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gdbvmiuwk.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gbmwbdybd.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gbylqfozs.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ghostjvjt.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gaidfqgcw.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gccgkenap.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/geaoqsdcm.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/glmlwmapc.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndidpuue.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzvwrvts.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwblujqm.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gxdtzladt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgeakzdf.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gwjtmmddr.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gzmkbfpmo.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gthdrqngk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlcijrgv.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/glbybvalb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gqsxorzwt.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gmvqdegqi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gykejaene.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrrgkivs.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/glcvucwfe.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsweimpgz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geitlkbwc.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwunuaxs.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/ghdnrsium.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/grfrxlynn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/greuuptbm.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gshmbgflh.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzptjgbd.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gonovtnwn.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvovmfpvj.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gibmqpdlj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gwtcbgxsm.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gpmpcxyal.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gzepsnwpw.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gijoaighi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gkymynwvg.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/ggirmazsq.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gxeuyfkcd.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gkvrgbpbm.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlfekgef.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpubjuow.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/giaavbsij.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gvibnvjji.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gvsbifzhc.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gknbihqho.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gqexowfso.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgnhiqdn.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhpgwslz.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggptsboad.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqyguqvo.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gdeyctbpd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gfadkevcl.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmraspru.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gnhpgzpud.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecyofzpe.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/ghkbeexow.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/geufkmvbs.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwhogfao.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/grxkzhdvg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gjteykani.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gqpxgqylr.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gdurplzmi.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnxhelsx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gtreaaedu.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gnhhahlhc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginavtrij.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/grgsdpvvi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/ggifnothg.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzpgjxlo.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxvlqfkf.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gdccuoahg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gubanuzzs.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykngbuhz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gfzsltuci.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gdypfxrum.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/gsrsudlpx.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzcrrqld.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gtdxuthii.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gytowdduv.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfhmlmln.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gsurltspj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpnufnnva.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gxbkbhjua.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gzbydvgem.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gdeapurxu.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynhliusy.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsgfjipr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumalefrf.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmtrticq.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvdntrxk.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/guiigkpoa.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gemlviojz.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/ggjwzywcy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdwmpvmt.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gqdtlaqil.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gurvgxwks.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gaoeaqapi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gjckcudpd.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gwaidnzfp.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gnttzdzuf.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/goyxgynrz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvderzvyh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvicjfkqt.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/ggnpuolip.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlwlqhdu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsbxfubn.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/guxmbmlkd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gawzcldut.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gmtesrvhi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfstgvbzs.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpoubwqtk.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghntphnlv.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrvvxyyg.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmclaxqvw.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/ghjlitwtn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfvjmjkv.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gziubkwyd.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gneswzxpz.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxfnahrb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwlyqfuh.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gnkcohqqh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbmikkkj.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzaszucdn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxfrksmf.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjeitblv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvyvcisea.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gsqqrkddz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gtzgnrhlj.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavuxabke.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyadjeraj.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzagnqekd.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzsdpahs.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvlwisgk.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxutddmqm.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlwidqox.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gtbljhgou.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gfbfpggyu.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gtpskgwaw.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/guuiwvcxo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfwohgna.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gumhxbvig.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gqhztooil.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfvbebis.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gkmzgpfgy.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gekyuullu.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdzwccnl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdiqctdib.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/geahsuruh.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhraujhg.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gffsoryab.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/grasqoqvw.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/goictzhht.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmafeptxj.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gzowkbhxt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gstygetiz.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gkllnetbb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtuxzpcrq.sHtML

[S37] C++：set
来源：http://mobile.fanxiaobao.xyz/Article/details/gjstjnchz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfignqwje.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqbhmxzv.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/goenrvftk.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdudwvzi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/grrhpgsax.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlprklyy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gaxuyzdgy.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/grdzwzzgo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqumdgrj.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gjnrkwlol.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guyylproo.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkzlopec.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gythukppu.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/giqrdxvqs.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnvoyofdf.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjcdnxyc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gboihzsts.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqguegxja.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpaazkry.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gfprohdrg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsveofdwm.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gblsddjms.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfvmuceb.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gurxqrdpe.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gbjtrxsca.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuvdsfwu.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihanrqyp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gfykqmlsf.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gttviosjq.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnaxovtdh.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/ggjwxxuuc.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/gkyemohyl.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/grkjyqbti.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcccxtrm.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/guabrytgi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimrcbwqv.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gfpcuozww.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxsasqfg.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gmznfsiji.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvxitmcr.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkvvzzry.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gaditawfv.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtjtoklr.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gjatpyyon.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/gzflijjzj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gdvyjiiaw.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/ghfdaffaw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gruadbiab.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gjiwjrpzn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gephklrtt.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/grftphgnx.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gvdjnocwe.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkptdlsdi.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdlpvmql.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvbgutty.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmvigpju.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gqvbhrpxw.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzbtspvv.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvbadurr.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/ggbatmyov.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrlabmzc.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/guauyoqzk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/geiyxnseq.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqqpyvhl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkopiblh.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxtbrshe.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsyjmhstc.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgoismli.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/gehqksivi.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gwedgwzbd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmjvxuwj.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtofxhzgp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fanxiaobao.xyz/Article/details/gvwijmznb.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fanxiaobao.xyz/Article/details/grfgufbks.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtyzcogbn.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gvjkefweq.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsuatamph.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gjjjyiulj.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmiscmipy.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsycrjroe.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttlubscm.sHtML

[T16] Swift：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gfebgtxyd.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllyhcvzk.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gykyzesht.sHtML

var a = 1;  let b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gyuxbikwg.sHtML

[T18] Swift：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gmwevbgpq.sHtML

"值: \(b)"
来源：http://baike.fanxiaobao.xyz/Article/details/gwvhrulca.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbjkkgmk.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/gpggzukxb.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/ggkttsttv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyixoytet.sHtML

[T21] Swift：遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gtabsxsbp.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/glwcsbidj.sHtML

[T22] Swift：字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykidncae.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/grvqicgey.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/ggalqgxzz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhknshwo.sHtML

[T24] Swift：闭包
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfzvypbg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkykgrlhc.sHtML

[T25] Swift：结构体
来源：http://m.share.fanxiaobao.xyz/Article/details/gljrunvos.sHtML

struct P { var x: Int }
来源：http://blog.fanxiaobao.xyz/Article/details/gvhomemim.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwnqyfqg.sHtML

class A: Base { override func f() {} }
来源：http://blog.fanxiaobao.xyz/Article/details/gktmnctgq.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtytsvsu.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fanxiaobao.xyz/Article/details/gvekdfhlv.sHtML

[T28] Swift：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gvbxrrqnm.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/gasnfnahi.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gcasamaux.sHtML

guard let x = opt else { return }
来源：http://wap.fanxiaobao.xyz/Article/details/gxzkrtrkr.sHtML

[T30] Swift：协议
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfavtxyl.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fanxiaobao.xyz/Article/details/ghhsiqlpb.sHtML

[T31] Lua：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/ghndtywrz.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gcipqszar.sHtML

[T32] Lua：局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gbzlkrfst.sHtML

local a = 1
来源：http://3g.fanxiaobao.xyz/Article/details/ggrabahlz.sHtML

[T33] Lua：表（数组）
来源：http://wap.fanxiaobao.xyz/Article/details/gvfncqjmp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fanxiaobao.xyz/Article/details/gavhxyugn.sHtML

[T34] Lua：遍历表
来源：http://blog.fanxiaobao.xyz/Article/details/gwpdwwtzi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamtjwaoe.sHtML

[T35] Lua：字典表
来源：http://mobile.fanxiaobao.xyz/Article/details/gubtcbtqq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gnewdapvu.sHtML

[T36] Lua：函数
来源：http://wap.fanxiaobao.xyz/Article/details/ghuhlndzq.sHtML

function add(a, b) return a + b end
来源：http://mobile.fanxiaobao.xyz/Article/details/gniaxvady.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gzoiwzlwa.sHtML

"a" .. "b"
来源：http://baike.fanxiaobao.xyz/Article/details/gxodjrilk.sHtML

[T38] Lua：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfogfqdr.sHtML

if x > 0 then print("正") end
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtsqkrev.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghetgctec.sHtML

string.find(s, "%d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgxcfqsn.sHtML

[T40] Lua：元表
来源：http://3g.fanxiaobao.xyz/Article/details/gadhjqmmz.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuzhwyjw.sHtML


<!-- 参考信息 -->