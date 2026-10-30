代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/gfkgyhdsx.sHtML

[R24] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gumqgaeqc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/geyyqfbns.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fehbvm.com/Article/details/gdepjsvga.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.hesvh.cn/Article/details/gcnbsalsw.sHtML

[R26] 命令替换
来源：http://blog.zdbjq.cn/Article/details/gkhuibbxd.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.hesvh.cn/Article/details/gmsauzyld.sHtML

[R27] 算术展开
来源：http://m.share.hesvh.cn/Article/details/gayjjrgqa.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.zdbjq.cn/Article/details/gshbgiptx.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/granibxwh.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/gjultvavi.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gwefdbpvr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fehbvm.com/Article/details/gcfssucfb.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/ggnycemse.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/gggefykzp.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/grivedeqg.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fehbvm.com/Article/details/gmtfnbmmm.sHtML

[R32] 参数个数校验
来源：http://read.share.zdbjq.cn/Article/details/gjmpvdkdf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gsysrhyzc.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/gjjsevwsv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gizzkcxuo.sHtML

[R34] 退出时清理
来源：http://www.blog.hesvh.cn/Article/details/gzahjtpwl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/ghkpgpjad.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/ghjbyefbg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.zdbjq.cn/Article/details/gnhhxtfbl.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/ghfxkhkit.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fehbvm.com/Article/details/gcmvlumhg.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/gwzqwudji.sHtML

files=$(ls -1)
来源：http://www.share.hesvh.cn/Article/details/grhgimydk.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/gfchjcukc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/ghiziovxr.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fehbvm.com/Article/details/gkpjbuked.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/geeuerjsg.sHtML

[R40] 追加写日志
来源：http://www.share.zdbjq.cn/Article/details/gjrssnhkt.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/grermhcar.sHtML

[R41] 丢弃输出
来源：http://baike.fehbvm.com/Article/details/gcygyfuat.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/gaayiisje.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/gmicunaec.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/gxzdvezsm.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/govtruoxx.sHtML

find . -name "*.log" -type f
来源：http://baike.hesvh.cn/Article/details/gtbmypkpf.sHtML

[R44] 按修改时间查找
来源：http://www.share.hesvh.cn/Article/details/gvtfwxvcq.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/gisqutdah.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/gtlzyqegc.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/gxekixmay.sHtML

[R46] 递归替换文件内容
来源：http://3g.zdbjq.cn/Article/details/gobqnfgxp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fehbvm.com/Article/details/gjztpyvup.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/gkepynorw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/gfmqcecwm.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/gjuvlqero.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gyvzffiag.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/glwnkyyuk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gcybgzwhh.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/gldggulcu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gfqllatfk.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/gypmapvku.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gdemqerbb.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/ggndqqual.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/gyzotgejk.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/gwzpselek.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fehbvm.com/Article/details/gqtqrflim.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/gnaustrcg.sHtML

diff a.txt b.txt
来源：http://mobile.zdbjq.cn/Article/details/ghgdrqupz.sHtML

[R55] 压缩与解压
来源：http://read.share.hesvh.cn/Article/details/gqsjqxbiz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.zdbjq.cn/Article/details/gxhydmjoz.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/gjooxrbev.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/ggjjgjxls.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/ghqzknpmw.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/gebqcbiok.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/gwlbkgckm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/gstuyteug.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gwrftrrnz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.zdbjq.cn/Article/details/gzudcjbid.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gitseynqe.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.hesvh.cn/Article/details/gthupcfiu.sHtML

[R61] 磁盘占用
来源：http://www.share.fehbvm.com/Article/details/gglfxfbom.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/gtbbafpjh.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/gbqalzftq.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.hesvh.cn/Article/details/guydtobyf.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/gaafirtpe.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/gmnhjbeoo.sHtML

[R64] 结束进程
来源：http://read.share.fehbvm.com/Article/details/gyquumotc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/givibmzgp.sHtML

[R65] 查看端口占用
来源：http://m.share.zdbjq.cn/Article/details/gkfrwvxnx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gzkipqdry.sHtML

[R66] 定时任务
来源：http://baike.zdbjq.cn/Article/details/gqkpvqibi.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/ghwglbyus.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.hesvh.cn/Article/details/gpeazentg.sHtML

openssl rand -hex 16
来源：http://3g.hesvh.cn/Article/details/gvcqpgkvn.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/gerezisfo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.hesvh.cn/Article/details/gotodbitd.sHtML

[R69] 生成随机密码
来源：http://www.blog.hesvh.cn/Article/details/gtpzjnabd.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.hesvh.cn/Article/details/ggczmiirp.sHtML

[R70] 时间戳与互转
来源：http://www.share.hesvh.cn/Article/details/gaeduyxzv.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gbadyabis.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gwnokbohy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/gkxaoqbfi.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gvwrhtgcf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gnowmodnk.sHtML

[R73] 分割大日志
来源：http://www.share.fehbvm.com/Article/details/gohtskfzp.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fehbvm.com/Article/details/gntkqtnmz.sHtML

[R74] 批量重命名
来源：http://m.share.zdbjq.cn/Article/details/gsaewqwwa.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/gnfzenynr.sHtML

[R75] 导出环境变量
来源：http://mobile.hesvh.cn/Article/details/ggjpgvmgs.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.hesvh.cn/Article/details/gxjoghsoe.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/gxonzfgyu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gmetseykh.sHtML

[R77] 读取用户输入
来源：http://read.share.fehbvm.com/Article/details/goulhzrzl.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/gjuveeinh.sHtML

[R78] 交互式菜单
来源：http://blog.fehbvm.com/Article/details/getvntbps.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/ghdnxhgny.sHtML

[R79] 解析命令行选项
来源：http://blog.hesvh.cn/Article/details/gepvnfizf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/gdeqpjesm.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.hesvh.cn/Article/details/gnhvcqhcy.sHtML

time ./run.sh
来源：http://wap.zdbjq.cn/Article/details/gyhillheb.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gizvuawmw.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/gflbcswdm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/golujulpu.sHtML

[S01] C：Hello World
来源：http://mobile.hesvh.cn/Article/details/gclvsqqmz.sHtML

#include <stdio.h>
来源：http://blog.fehbvm.com/Article/details/gsczshnvo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/gcoksqrgq.sHtML

[S02] C：变量与格式化输出
来源：http://3g.zdbjq.cn/Article/details/gnrwnoilj.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.hesvh.cn/Article/details/gunbrozhd.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/gubeasiba.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fehbvm.com/Article/details/guqpjeccv.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/geavedzfd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.hesvh.cn/Article/details/gvdgaoryh.sHtML

[S05] C：字符串长度
来源：http://3g.hesvh.cn/Article/details/giegvirdc.sHtML

strlen(s)
来源：http://baike.fehbvm.com/Article/details/gkppmjvzw.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/gjvzfljtl.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/gytbasrdm.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fehbvm.com/Article/details/guhhmaxdk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/gmmzciqmg.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.hesvh.cn/Article/details/gxglrzolw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.zdbjq.cn/Article/details/gzldspcmr.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.hesvh.cn/Article/details/gcxznqbhs.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fehbvm.com/Article/details/glfwlrxaj.sHtML

[S10] C：指针与解引用
来源：http://read.share.fehbvm.com/Article/details/goxsxuzxz.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fehbvm.com/Article/details/gymnwnzwd.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gepsykdxr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/gwmasjtqv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.hesvh.cn/Article/details/gcklevjam.sHtML

fclose(f);
来源：http://blog.hesvh.cn/Article/details/gobsdezio.sHtML

[S12] C：写文件
来源：http://baike.fehbvm.com/Article/details/glqkjkjlu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.hesvh.cn/Article/details/gzsubqjsu.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/gqjxeebth.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/gppccdcvt.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/glmrwectn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/gatgspwjw.sHtML

[S15] C：类型转换
来源：http://m.share.fehbvm.com/Article/details/gkkcrpozw.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/gjlzalrxo.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/gnmppmemp.sHtML

x |= (1 << 3);
来源：http://read.share.zdbjq.cn/Article/details/gzybibrvh.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gbzxonymo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/gbkrkqgqw.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/gnzuoymfd.sHtML

int main(int argc, char **argv)
来源：http://blog.zdbjq.cn/Article/details/gvlkkrstw.sHtML

[S19] C：快速排序
来源：http://mobile.zdbjq.cn/Article/details/gxggpayvh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gpjzwrkoz.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/galurwtcl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gqcwmtrfp.sHtML

[S21] C：字符类别判断
来源：http://3g.zdbjq.cn/Article/details/gtcygvrvp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.zdbjq.cn/Article/details/gvueaivmt.sHtML

[S22] C：字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/gvxsihbfl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/gkffzhhky.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/glcmgwuez.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gyhfnxmlb.sHtML

[S24] C：获取本地时间
来源：http://wap.fehbvm.com/Article/details/gmyjqsgnm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.hesvh.cn/Article/details/grsjyxfcq.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/gofkxsqkb.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/gfkynvuds.sHtML

[S26] C：内存清零
来源：http://m.share.fehbvm.com/Article/details/gbezmhwwr.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.zdbjq.cn/Article/details/ggucttwyn.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gngduxaip.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gpuymmvhj.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/gvlbqlvgm.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/ggktdlzll.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/gdqjhhbry.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/gccbtubex.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/ghltvdztu.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/gllgnzjte.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/gpkvbrfsp.sHtML

#endif
来源：http://www.m.share.zdbjq.cn/Article/details/gkwnoiwgq.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/gqkvdagbl.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/getxpkbfs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/glwfkxxgx.sHtML

[S32] C++：字符串
来源：http://blog.hesvh.cn/Article/details/gbyflqaii.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gmolzfhvb.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/gpifjoeqg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gzruizxsj.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/glhdngfam.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.zdbjq.cn/Article/details/grunfwqiz.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/glsiqhiaz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/goagddbva.sHtML

[S36] C++：unordered_map
来源：http://wap.hesvh.cn/Article/details/gcpsldwkm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gstdrtvip.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/gdhafwqke.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/gqnqcuklm.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/gbsthuxuc.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/gzygyuhno.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fehbvm.com/Article/details/ghggtcmab.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.hesvh.cn/Article/details/gdtrbxlxq.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/ghhbnhlwc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fehbvm.com/Article/details/gmmiluwwe.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/geazxkaud.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.zdbjq.cn/Article/details/gckthimvk.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.zdbjq.cn/Article/details/gcilzgbuk.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fehbvm.com/Article/details/gwtfwfptf.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/gtgcpolxg.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/gkbhsyrlx.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/gsddsmcme.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqzcwntwm.sHtML

[S45] C++：lambda
来源：http://baike.fehbvm.com/Article/details/gdwrggnao.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.hesvh.cn/Article/details/gtqmfqmfn.sHtML

[S46] C++：函数模板
来源：http://mobile.fehbvm.com/Article/details/gbqtvbcts.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/gomrgaqmb.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/gwvjmmhyl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/guxacqagl.sHtML

[S48] C++：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gpvdhscth.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.zdbjq.cn/Article/details/gsuzcfiwh.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/gyslkqqlr.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/gzshkudaa.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/gmoexwnyg.sHtML

[S50] C++：格式化数字
来源：http://www.share.zdbjq.cn/Article/details/gxguojmdq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gxxzlaejl.sHtML

[S51] C++：显式类型转换
来源：http://blog.fehbvm.com/Article/details/gbfcshcce.sHtML

static_cast<double>(a) / b
来源：http://m.share.fehbvm.com/Article/details/gztxfkqew.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/gsjvlwoal.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fehbvm.com/Article/details/gfkbsrfxl.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/gmtfxuvlg.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fehbvm.com/Article/details/gutqrszvz.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/gtfqywirp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/ggjzsiznf.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/gxrcylktk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/gmlrrgajm.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/gzqwdshdv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.hesvh.cn/Article/details/gtfgpyely.sHtML

[S57] C++：编译期常量
来源：http://baike.zdbjq.cn/Article/details/genvgyyud.sHtML

constexpr int N = 10;
来源：http://3g.fehbvm.com/Article/details/gfrgzcvmf.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fehbvm.com/Article/details/genmvfudn.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.zdbjq.cn/Article/details/gwbahrxml.sHtML

[S59] C++：静态断言
来源：http://read.share.hesvh.cn/Article/details/gtxtszhsv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/gbywwcbbw.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fehbvm.com/Article/details/gtihobaij.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fehbvm.com/Article/details/ghhrzhozo.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxlvvcndr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/giyzdeemr.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmakacrkb.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/gijhjuosf.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gefacqhid.sHtML

[T02] Kotlin：变量
来源：http://m.share.fehbvm.com/Article/details/gboyhztem.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.hesvh.cn/Article/details/gfkcuaqja.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/gqvltmlit.sHtML

"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gegscgwij.sHtML

[T04] Kotlin：空安全
来源：http://3g.hesvh.cn/Article/details/gfvvyuqlj.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/gmoljqcur.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/gygdwyyzl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/girwtopbu.sHtML

[T06] Kotlin：集合映射
来源：http://baike.zdbjq.cn/Article/details/gcqerxsqe.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/giyxlvbig.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gwhjqiupc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/ggczmehwj.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gzdjvhkwr.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gljblzqmm.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.zdbjq.cn/Article/details/glesoawjd.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.zdbjq.cn/Article/details/gfxhvwbzb.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fehbvm.com/Article/details/gjpvxochb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.hesvh.cn/Article/details/grqmqlypg.sHtML

[T11] Kotlin：协程
来源：http://wap.fehbvm.com/Article/details/ghvwvtrrt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fehbvm.com/Article/details/gzseqmjls.sHtML

[T12] Kotlin：解构声明
来源：http://baike.zdbjq.cn/Article/details/ggthsofvt.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/ghuffnjbv.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/gyablkxys.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/gjovkxndg.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/gasiulcpp.sHtML

for (i in 1..10) println(i)
来源：http://wap.fehbvm.com/Article/details/gkpfymjiu.sHtML

[T15] Kotlin：接口
来源：http://m.share.fehbvm.com/Article/details/gnnpcaqjd.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fehbvm.com/Article/details/gopwsrbxq.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/gsrbmoirv.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gxtdmuvxf.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/gcgtqqfzp.sHtML

var a = 1;  let b = 2
来源：http://www.blog.hesvh.cn/Article/details/ggxcwvvad.sHtML

[T18] Swift：字符串插值
来源：http://3g.hesvh.cn/Article/details/glmbntlgb.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/gfjbscsjc.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.hesvh.cn/Article/details/gmkywmbpz.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/gdffymhgm.sHtML

[T20] Swift：数组操作
来源：http://blog.hesvh.cn/Article/details/grkzwnkxs.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.zdbjq.cn/Article/details/gialmzwgt.sHtML

[T21] Swift：遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gbjszarvw.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/gtjpuglpy.sHtML

[T22] Swift：字典
来源：http://3g.fehbvm.com/Article/details/gmuvbgodr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.hesvh.cn/Article/details/gavmmmygw.sHtML

[T23] Swift：函数
来源：http://3g.fehbvm.com/Article/details/gbjydznzg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fehbvm.com/Article/details/ghwbsajld.sHtML

[T24] Swift：闭包
来源：http://wap.hesvh.cn/Article/details/gtwfmxpuw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gryqzvsru.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/gvbmkjzyt.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/gcszoxksa.sHtML

[T26] Swift：类与重写
来源：http://baike.fehbvm.com/Article/details/grkdmqimb.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gmsootbnd.sHtML


<!-- 参考信息 -->