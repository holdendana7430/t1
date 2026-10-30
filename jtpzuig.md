代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgjvexmg.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/govcjefxc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlpwcqbi.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcowzrjq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgrvikse.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/griphoxmn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/glamderdf.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gqsrphjtn.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotzalbgb.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gapyrwxig.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gnovlgsup.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gvewhhker.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gayquhcqj.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgcaaraj.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkrkeikd.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gagaiqdtt.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhqzcvca.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/ggoqeglgc.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxjqrtzd.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/giooemqsg.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/ghwpxobwf.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gohtjjiox.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdkoulhy.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gfemyvigi.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzzqykil.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/ginwsafbc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gaziirdni.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtxheeln.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gyelrmqka.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlprjyyj.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmrkzdtr.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrxxwqwe.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gvdtseejt.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/glfnnhvxg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlmukotv.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbtoznsv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gvwmogixq.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gejwvwdkw.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/ghwkpdccz.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrxfnvpn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrwuiexs.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gkqoztedf.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/glsvyabfi.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaekqgywp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjdfeerg.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/goyrfyukk.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gaaggmklo.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gawpbmtmd.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhdmeuei.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gpfiwdaej.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbebhzpv.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gicbqnbfx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gytrduhkn.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/govuwtlti.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/guywtbpmt.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/glymmwqyp.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjxgeuqh.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gjywmnovr.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gnohmaiyt.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gluuwxudm.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpzijqca.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqchdopiu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvdjyehg.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/goqrwkamv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gdphvxhey.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/ghfdifrun.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/glwkmdyij.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gtuvvxylf.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gdknuhqou.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gvfamiwmw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gauzdzawt.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gswxqolkt.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwfyklpu.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/ggnsbjsfr.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gerljqcte.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhtvzpnm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gdcomdpuu.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gmhmmecxh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gkidlqxnm.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxokqiixb.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gkdwfvsry.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gvpyvjafy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giudkdsem.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gfordhehl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gifaizjzn.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgaakelw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnapwlcts.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gbehishho.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gbfzsvumq.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/gvopjxzml.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gwrirefmx.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/ghtlgcpyw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gaarwjfpp.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfybvxuz.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/ghggjuiwy.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwlgafvz.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/guazotpdz.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjslzgfm.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdprmtjo.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakygvllj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/gouawfbcl.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gzntcdhbu.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/ghmbuswed.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/giqmzpfyi.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/gscervxhg.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gldmopocq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/glctftuvn.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrzdwxbm.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gxoylugqk.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/ghblagqft.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gfoibidzr.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvqsxcqs.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gddqlyqvh.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpoqgdmin.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/gujbdxoxf.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gueslcfyz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrrvhopi.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhfehxod.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/ghrxvbkng.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gjvdwyehi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjsaehvp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfobywflc.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gpuilplcs.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gywidyqth.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/goqnbtata.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrmgczmk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gotgslvrh.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gxiamwadl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gsvtbbmdy.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gmshnsdki.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gwuwjkoyk.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gmorsgdyt.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjddkonnc.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gepdurawr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/ggmsnsgot.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/grknmdmxr.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfweyiowo.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/grildnufp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrpmldgg.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gbynmjkyz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/ggeopfsgu.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpgeyytm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbudjjyng.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gmhcpxzns.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/ghuihslee.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gfgnrckuf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgbembzr.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gnadgtwrt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gbdfjhzhj.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkomrjfnk.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gfbsfcucw.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gijyydvxn.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvqxnjen.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznnmflqc.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnczxwjad.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwjhmafk.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gwadejvnd.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gywlzgmwp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnujunrdr.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgpglyvb.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkadgbsf.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gobdbkoei.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrrttczo.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gsrvjwvom.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gtijomsuo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpheiquby.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gotuisqlv.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gdzyonepr.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsskabur.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbmlcamz.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gaevxtpkk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxukhniz.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/ggugjsevm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/glptyvzab.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzolhvvw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryvwxibw.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtqsnqhd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/guhsbltkg.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/gooojxjdj.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifvcifkw.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxhfaeda.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gclwaigkl.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gygfdnsue.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gnizpjkya.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gavgkmcom.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gckgiapzh.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gsabezqsa.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmyxibana.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqovfajl.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gbyfxehfi.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gpehdxjtc.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvshjcxie.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaedapexf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gajpkxgnw.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhbjxmeb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhijkpqr.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gokrwxzxq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmedzouea.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gmaaumidx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/goyqpdqez.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gwdcbqrse.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gkxsxqmvl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gywietvex.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/gltyomqae.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gacloefyl.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhtrzomy.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gimzijhzn.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqfclquu.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvmgjgeed.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gigolzrnu.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/ggbnsdljx.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltvwzjbg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gdsmilges.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdfqebnz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvdbzhlg.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gnrjwlobf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnpqvdaso.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gcedlmzhh.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduyipmre.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gbxbneiwl.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gyqsehzce.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/gphclctbf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gyytzrprx.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmbyrflc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqlgmvjr.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gpznfpjwh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/giprlrelu.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ghcbdzlqd.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gylkejxfg.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucpnexxq.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gevkdlxzt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/grachswuy.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgqpgbfe.sHtML

"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/girsdhign.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlvumoeb.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/guyesyhgm.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gtdwuscuw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gacxmlhop.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gjflngook.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gotznoaum.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhufmqym.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsiiwopob.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzvgozbn.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsiawznf.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnnovkxc.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gooohahwp.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fanxiaobao.xyz/Article/details/grunlqhtb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkyrgddz.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gebqebemt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fanxiaobao.xyz/Article/details/ghkzivwej.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrrdldsh.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccfwoklg.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxteocwg.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gefmjnfie.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxtyjank.sHtML

for (i in 1..10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/ggsfhneit.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/gqapfcizz.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gxolixqyy.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/grecaviyk.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gbffmrbtj.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyffekem.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gddcrrray.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/giirjzqga.sHtML

"值: \(b)"
来源：http://www.share.fanxiaobao.xyz/Article/details/guijixyoj.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/guuklwvje.sHtML

if let n = opt { print(n) }
来源：http://blog.fanxiaobao.xyz/Article/details/gpcjzejja.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqwqymlp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/ggngemnqx.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gawmidkxg.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghllfaqdo.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfldkkrao.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/grqgeehxa.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gtzgdtgnf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqcefeev.sHtML

[T24] Swift：闭包
来源：http://baike.fanxiaobao.xyz/Article/details/gefpjnyjb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbalhuqj.sHtML

[T25] Swift：结构体
来源：http://www.share.fanxiaobao.xyz/Article/details/golfqiunv.sHtML

struct P { var x: Int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzopytnqd.sHtML

[T26] Swift：类与重写
来源：http://wap.fanxiaobao.xyz/Article/details/gazfkjpwl.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfeppvqng.sHtML

[T27] Swift：错误处理
来源：http://m.share.fanxiaobao.xyz/Article/details/glmyfandi.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fanxiaobao.xyz/Article/details/glbjlixit.sHtML

[T28] Swift：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gswexkddc.sHtML

enum Color { case red, green }
来源：http://3g.fanxiaobao.xyz/Article/details/gwwdzzymc.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fanxiaobao.xyz/Article/details/gdykcdfcd.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gihlpufiw.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjrmiwzj.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gqqneoxnu.sHtML

[T31] Lua：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gdsmdjamu.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gvqwlkfvb.sHtML

[T32] Lua：局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gbfwfwcbd.sHtML

local a = 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gmoxjkfit.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpgljkpx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fanxiaobao.xyz/Article/details/gczwedjbm.sHtML

[T34] Lua：遍历表
来源：http://baike.fanxiaobao.xyz/Article/details/grnkgcddy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fanxiaobao.xyz/Article/details/gcbusyhtq.sHtML

[T35] Lua：字典表
来源：http://baike.fanxiaobao.xyz/Article/details/gaqjhpyjb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtienwrnf.sHtML

[T36] Lua：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gofslqwku.sHtML

function add(a, b) return a + b end
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrjdxxlp.sHtML


<!-- 参考信息 -->