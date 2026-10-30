代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.hesvh.cn/Article/details/girfeebzz.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/govhbzhij.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gcnqsqyeu.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/gcpphvwns.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fehbvm.com/Article/details/gkwnpjsah.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/ghcpflmtj.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/ghdmulukp.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/gfuuodjkf.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fehbvm.com/Article/details/gjpkwyeyh.sHtML

[R28] 浮点运算
来源：http://www.blog.hesvh.cn/Article/details/getoumfai.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.hesvh.cn/Article/details/gvghpqado.sHtML

[R29] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gruzgmvnt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.hesvh.cn/Article/details/gynmdolmf.sHtML

[R30] 函数返回状态码
来源：http://baike.zdbjq.cn/Article/details/gxtkpnrcf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.hesvh.cn/Article/details/gedwsnflp.sHtML

[R31] 局部变量
来源：http://www.blog.fehbvm.com/Article/details/gtdpwvyrw.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/gxsfoakzg.sHtML

[R32] 参数个数校验
来源：http://read.share.zdbjq.cn/Article/details/gyavbwnyz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gdfthyskc.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.zdbjq.cn/Article/details/gccguvomu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gaityhhnz.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gjzmjlcej.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gikscaizt.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gpbplllml.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.zdbjq.cn/Article/details/gzjkjrvlb.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/gsgcsnsam.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/gpsoihmcy.sHtML

[R37] 把输出赋给变量
来源：http://3g.fehbvm.com/Article/details/grmsvovlu.sHtML

files=$(ls -1)
来源：http://read.share.hesvh.cn/Article/details/gzvaxsvzj.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/gnnatdgcp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/gsogopogo.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fehbvm.com/Article/details/gtqtmjxxl.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gsklrzrwm.sHtML

[R40] 追加写日志
来源：http://3g.zdbjq.cn/Article/details/ghurzrzhx.sHtML

echo "log" >> out.log
来源：http://wap.zdbjq.cn/Article/details/gxezttgdy.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/gwnazeeah.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gntsysdzs.sHtML

[R42] 输入重定向
来源：http://www.share.zdbjq.cn/Article/details/gumqrukwb.sHtML

wc -l < a.txt
来源：http://baike.zdbjq.cn/Article/details/gtnhmoxxo.sHtML

[R43] 按名字查找文件
来源：http://mobile.hesvh.cn/Article/details/giriisxck.sHtML

find . -name "*.log" -type f
来源：http://m.share.hesvh.cn/Article/details/golyfydlm.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/geiuxftfv.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/gidgplhcn.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/gtcaoyxpl.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/ghncruyxs.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/gkpspjces.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fehbvm.com/Article/details/gwpizkttp.sHtML

[R47] sed 单行替换
来源：http://www.blog.zdbjq.cn/Article/details/glywajqtc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gnpxahtnj.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fehbvm.com/Article/details/gyammjgqf.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gxvqrqkcs.sHtML

[R49] awk 带条件
来源：http://m.share.zdbjq.cn/Article/details/gcirpqjws.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fehbvm.com/Article/details/gdtnheiyj.sHtML

[R50] awk 求和
来源：http://www.m.share.hesvh.cn/Article/details/gsmfyrttw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fehbvm.com/Article/details/ghfnhgbyb.sHtML

[R51] 排序去重取前几
来源：http://blog.hesvh.cn/Article/details/ginfimvvf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.zdbjq.cn/Article/details/geaxzhgwx.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/gdpnbkxor.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/ggqouaysd.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fehbvm.com/Article/details/ghnshyeqd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fehbvm.com/Article/details/ggkubwdni.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/goravsucp.sHtML

diff a.txt b.txt
来源：http://wap.hesvh.cn/Article/details/gitzsbyid.sHtML

[R55] 压缩与解压
来源：http://read.share.fehbvm.com/Article/details/gsiyodqan.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.zdbjq.cn/Article/details/gjqcacizv.sHtML

[R56] 远程拷贝
来源：http://m.share.hesvh.cn/Article/details/gcdsfawqi.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/glznqessk.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/ggxzyupoy.sHtML

ssh user@host 'uptime'
来源：http://baike.hesvh.cn/Article/details/gdlerbalt.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/gkpqbgtbg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/gpkcltmvh.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/gvtacaaxr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/gjjhfxdmi.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gegpmkrnf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/gsmsihyvv.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/glbrcyana.sHtML

df -h;  du -sh *
来源：http://www.m.share.zdbjq.cn/Article/details/gsrwtqfqx.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/gzhrgqnic.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.zdbjq.cn/Article/details/gvmzvajta.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/gceedctkk.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/grhyzvhii.sHtML

[R64] 结束进程
来源：http://wap.hesvh.cn/Article/details/gbtwtyhbc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.hesvh.cn/Article/details/getnsrhvp.sHtML

[R65] 查看端口占用
来源：http://baike.fehbvm.com/Article/details/grkehupti.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/gzfhhssxd.sHtML

[R66] 定时任务
来源：http://mobile.hesvh.cn/Article/details/gkouhlypx.sHtML

crontab -e;  crontab -l
来源：http://blog.fehbvm.com/Article/details/geywsrgrk.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/gzzzdoscr.sHtML

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/gltisuotg.sHtML

[R68] 计算文件校验值
来源：http://3g.zdbjq.cn/Article/details/gwtribmcd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.hesvh.cn/Article/details/gfekzfsrz.sHtML

[R69] 生成随机密码
来源：http://read.share.hesvh.cn/Article/details/gjkasxhzz.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.hesvh.cn/Article/details/gdcefdqba.sHtML

[R70] 时间戳与互转
来源：http://read.share.hesvh.cn/Article/details/gjuqgkcpe.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/gjqexirgt.sHtML

[R71] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gaptcsvqu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gcgvolhcn.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/gifzdxiyz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gcowuukky.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/gubrdsrzl.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/gfpqdihes.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/ggpdibwtn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fehbvm.com/Article/details/gyhndjizf.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gfgyukwxa.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/glxasvvjy.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/gehphtxfx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gznizdkwh.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/ghlbiwowg.sHtML

read -rp "请输入: " ans
来源：http://baike.hesvh.cn/Article/details/gablgycwl.sHtML

[R78] 交互式菜单
来源：http://blog.fehbvm.com/Article/details/gjapqivjx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.zdbjq.cn/Article/details/gmfvsetrx.sHtML

[R79] 解析命令行选项
来源：http://m.share.fehbvm.com/Article/details/gwkuozqgn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fehbvm.com/Article/details/gjptkwcxg.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.hesvh.cn/Article/details/ggsesoeuq.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/ghsehvroo.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjzeebwno.sHtML

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/gsryotfcu.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwusjppgp.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/gqskgsvum.sHtML

#include <stdio.h>
来源：http://wap.fehbvm.com/Article/details/grunnzcjq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/guoqdngmx.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gsilrzxuo.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.hesvh.cn/Article/details/gyrgdqhoo.sHtML

[S03] C：读入整数
来源：http://m.share.hesvh.cn/Article/details/ggcyzdwrg.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/gyysjhpdi.sHtML

[S04] C：字符串复制
来源：http://m.share.zdbjq.cn/Article/details/gvgqshxoc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.zdbjq.cn/Article/details/gofguvxqn.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gezbvktpg.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/gqtewmqmx.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/gzjarxlxo.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/gtwkqwbmz.sHtML

[S07] C：数组遍历求和
来源：http://3g.hesvh.cn/Article/details/gjhcjyxxf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/gyltiskia.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/gbzphgtsv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/gqtiurqso.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/gzqglqgio.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/gynzdcncx.sHtML

[S10] C：指针与解引用
来源：http://wap.hesvh.cn/Article/details/gethbkvyd.sHtML

int *p = &a;  *p = 5;
来源：http://baike.zdbjq.cn/Article/details/gwwhqhspo.sHtML

[S11] C：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gvnpqynvm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/gqqfletlf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gyqzebrth.sHtML

fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gsewqqiya.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/gosjlslhv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/grtsdvboa.sHtML

[S13] C：宏定义
来源：http://www.share.zdbjq.cn/Article/details/gjhiozhhr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.zdbjq.cn/Article/details/guqayoltj.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/gnqfzyowp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/gbxukhcgg.sHtML

[S15] C：类型转换
来源：http://www.m.share.fehbvm.com/Article/details/ghmsndnmk.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/gmpstpacp.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/guqpcoxnm.sHtML

x |= (1 << 3);
来源：http://wap.fehbvm.com/Article/details/ghvsycfui.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/gkarrwsda.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/gsdeemwqc.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/gpuqadhfu.sHtML

int main(int argc, char **argv)
来源：http://mobile.fehbvm.com/Article/details/gckkefnjp.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/guuuegrqu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gpvhbglqh.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/gdybooxap.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gtenawhit.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/gdamhfcma.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.hesvh.cn/Article/details/gwkjomryg.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gbgwwhvnt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/gtchmeham.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/gdolrxrnh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/gcmsgnhjs.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/glnlwxfws.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/gqafsshzp.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/gpjaqmtso.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/gzvswepel.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/gtwiroksn.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/gexjqepxu.sHtML

[S27] C：定义常量
来源：http://3g.fehbvm.com/Article/details/gzqhrnltv.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gxldpvrxf.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/gqcbsdawh.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/gxasmlaxm.sHtML

[S29] C：变参函数
来源：http://blog.zdbjq.cn/Article/details/gvjpranlu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/gxlfdjyvq.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/gvzfyoewl.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/gdulbptlz.sHtML

#define X_H
来源：http://www.m.share.fehbvm.com/Article/details/gkdnkztmx.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/gamgjyfhe.sHtML

[S31] C++：Hello World
来源：http://baike.hesvh.cn/Article/details/guwepiveg.sHtML

#include <iostream>
来源：http://baike.zdbjq.cn/Article/details/ggwydsrma.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fehbvm.com/Article/details/gneuezvbs.sHtML

[S32] C++：字符串
来源：http://baike.fehbvm.com/Article/details/gttgnhdsu.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/gueqxlyfe.sHtML

[S33] C++：vector 增删
来源：http://blog.fehbvm.com/Article/details/gpdzjmuyu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/gvzbicpna.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/gepqjrpua.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.zdbjq.cn/Article/details/gfjuegwkh.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/gmnuhpzto.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/glwdqrlcw.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/gkddltsmc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/guivtmhio.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/gtlqcgvve.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/ghxbcrumz.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/gmdoufidl.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gjlfjonbk.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.hesvh.cn/Article/details/gztwtgbyc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.zdbjq.cn/Article/details/gwprkesym.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/gxrkcfcpd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/gppzjewal.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fehbvm.com/Article/details/glicxvbau.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/glseyrvzn.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.zdbjq.cn/Article/details/gmhttikcf.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.hesvh.cn/Article/details/gsrcjucau.sHtML

[S43] C++：智能指针
来源：http://3g.hesvh.cn/Article/details/glgyfptso.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/grstscusj.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/gyqytandt.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gxtnyyttu.sHtML

[S45] C++：lambda
来源：http://baike.zdbjq.cn/Article/details/gtriwvnch.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/gpfxgjlvd.sHtML

[S46] C++：函数模板
来源：http://www.m.share.zdbjq.cn/Article/details/gkkkhabjs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/guueyvfzi.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.hesvh.cn/Article/details/gpyitwuut.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.hesvh.cn/Article/details/gykfbbimz.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gerpdbanl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/ggxxdwvui.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/ghvsvyogg.sHtML

[S49] C++：写文件
来源：http://mobile.fehbvm.com/Article/details/ggqyhnawv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/gikyqgpve.sHtML

[S50] C++：格式化数字
来源：http://3g.zdbjq.cn/Article/details/gfvhcebmn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gbtgzilfv.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fehbvm.com/Article/details/gvfohnded.sHtML

static_cast<double>(a) / b
来源：http://blog.hesvh.cn/Article/details/gkfjldbfl.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/gofjxirwa.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fehbvm.com/Article/details/gbfjhmeuc.sHtML

[S53] C++：移动语义
来源：http://www.m.share.hesvh.cn/Article/details/gerfipqjp.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.zdbjq.cn/Article/details/ghitlckgz.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/gicgxltsg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/gzwjragxm.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/gyygfibpq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.hesvh.cn/Article/details/gdupiddse.sHtML

[S56] C++：optional
来源：http://m.share.hesvh.cn/Article/details/giwlhnnvx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/gtrmpxuuj.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/gzrbradnr.sHtML

constexpr int N = 10;
来源：http://3g.fehbvm.com/Article/details/gyipnlqxr.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/ghkbrydqc.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/genhspidd.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/grdjxsgwz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fehbvm.com/Article/details/gytjwsjqz.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/gusosdrka.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/gjuzojhfz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqtgfnrjf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gctpihyry.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmtteytbq.sHtML

[T01] Kotlin：Hello World
来源：http://3g.hesvh.cn/Article/details/gbevshmnv.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gdvceobtl.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/gxhgtwkaw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.hesvh.cn/Article/details/grldtpepw.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.zdbjq.cn/Article/details/gknunainy.sHtML

"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/glcjyofpv.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/grzglbksq.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/gjpqrkpfr.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fehbvm.com/Article/details/gyxnofqjc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.zdbjq.cn/Article/details/gllpdjyrk.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gtsquveqv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/glciqauqc.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/gkvhapokn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fehbvm.com/Article/details/ggqsrdoes.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/gkmavztxa.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/gdzkyeecx.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/gnmnybbbv.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.zdbjq.cn/Article/details/gvuwviizc.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/ggjvterhd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/gxhbvuvgh.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fehbvm.com/Article/details/gxpnzlska.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.zdbjq.cn/Article/details/gttetzlow.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/gbsqxyafg.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gzmzbebzo.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.zdbjq.cn/Article/details/godtudlqo.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/gqqfmvqfo.sHtML

[T14] Kotlin：循环
来源：http://3g.zdbjq.cn/Article/details/godqfjoyh.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/grhlegjko.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.hesvh.cn/Article/details/gcmmeixcl.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/gxxmehqbj.sHtML

[T16] Swift：Hello World
来源：http://wap.fehbvm.com/Article/details/gndskonex.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gzogniwtq.sHtML

[T17] Swift：变量与常量
来源：http://baike.hesvh.cn/Article/details/gsqedugjb.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/gzyaadbny.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gfnovjwld.sHtML

"值: \(b)"
来源：http://wap.fehbvm.com/Article/details/gagocnqzb.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.hesvh.cn/Article/details/gajwhzvub.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/gqwziuyev.sHtML

[T20] Swift：数组操作
来源：http://m.share.fehbvm.com/Article/details/grdgeqfvm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gemapcyct.sHtML

[T21] Swift：遍历
来源：http://baike.hesvh.cn/Article/details/gfxdfjjtu.sHtML

for x in a { print(x) }
来源：http://www.blog.fehbvm.com/Article/details/gvtkzgyuf.sHtML

[T22] Swift：字典
来源：http://mobile.hesvh.cn/Article/details/guivkdveo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.hesvh.cn/Article/details/grhkyvxaw.sHtML

[T23] Swift：函数
来源：http://mobile.hesvh.cn/Article/details/gnokyrons.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.hesvh.cn/Article/details/gwyqkvygo.sHtML

[T24] Swift：闭包
来源：http://www.share.fehbvm.com/Article/details/gfikqlmex.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.hesvh.cn/Article/details/gzstwebdc.sHtML

[T25] Swift：结构体
来源：http://m.share.zdbjq.cn/Article/details/gzdkfzpxt.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/giypoqqol.sHtML

[T26] Swift：类与重写
来源：http://www.share.fehbvm.com/Article/details/gvsdctlgz.sHtML

class A: Base { override func f() {} }
来源：http://baike.hesvh.cn/Article/details/ghminzjkf.sHtML


<!-- 参考信息 -->