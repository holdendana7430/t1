代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gukbsjcsx.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/gtzcltuhf.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/gxytewmkc.sHtML

[R27] 算术展开
来源：http://read.share.fanxiaobao.xyz/Article/details/gapejocqk.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/geadqtcnx.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgnrmfcg.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gmmvtdgyz.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbjtsfkg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/gswhufcpo.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtmliebj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsixypbq.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gluiiqusg.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/goeawsvim.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gidcuefyn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdynhwiuz.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaubuqnmg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glusgxdul.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/gudjqmdgk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gmribpybk.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpaenofz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gbqnaiuxo.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gedngqqoa.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/gigpwmeso.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gnzrcfxsw.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gyoodmhml.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzvrfyzs.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gveysvrqw.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gafsedjcg.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/guklfkypv.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gklfngpnt.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gkhvafkdw.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/goupfqesm.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gqecnusts.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/goekfqbkz.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhwqlzjb.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/grsfbgjbr.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gbrweqyde.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gaiyszjhk.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gevtstztk.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gannritxw.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/ghsypoyvb.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gcyvelkog.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgnadfhb.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/ggudoypcu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfnhekgn.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokelksgb.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gxoeyksyf.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbahptftf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmyhmhth.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggadakoyn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhfrywca.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifphoyur.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhejwczz.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gjbkwyebk.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudcaotwo.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrzfzatx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/gqyajinng.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ghygwnprg.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbmoaqih.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gzoiuxhde.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/ggiymykhd.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gikggdqwc.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqzmfldq.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqqvamlr.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/guoxyxxvo.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gjdtoyvsr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/giasjvlor.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/ghztapzel.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gnihjfrwi.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gvumrssqa.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gviijfrcb.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gmqimwgsa.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gblrrwhdb.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gwouqkeda.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/grjlcxdlx.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfjbulty.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gaofxkful.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqdmlifl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gbrjxofdy.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/ggkwxdmyn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gqsxdcgxs.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gsjgsbzoc.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gdwjivnmr.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhitgqbk.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gprnmtmqd.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfwxkvwy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gishccxia.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gqjqgbqgp.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gordckznc.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyguhkul.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gaghvdhql.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gozuhbrih.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/gdujqdhtj.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgpymsta.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpervqilv.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthmajebb.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gzgnkuuis.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcciyezjk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtswnnime.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gzaxkmibr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvovzvss.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gkoswkjei.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gccyffdkw.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/glfyjxiyo.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/grcfqpdhh.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gagdqvazw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gzyqriizf.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmfulazy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gacfdnkmi.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdpvewyq.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gznxiuabi.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjhimzdi.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gscttnonk.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/guohxszji.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gdzcgiybp.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gapbvlyys.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwiipmxvg.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/ghbgouxun.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglxbkial.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gugwyahab.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/guhpqfkjy.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcydmumc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gcpmjvuqk.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gqahykpns.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gnqkakldj.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gzasqfpxa.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gdeenfgta.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/guqnizsmf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/graqkrhwt.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwaectrn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/ghwxytjeo.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlszvhlr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/guzivihvy.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/grpovkfhr.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdapikiwu.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypqxwgce.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvofwzws.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gmpembmij.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gywtwyvdk.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glibtdfjo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/geiilzscx.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmwlsnfk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzvkoyni.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdobymbf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmhprwfz.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gyphzhyhw.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/gxpckgmge.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunlftvgo.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gwpowvhlx.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gtbwwxbvk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/gjyvznqvk.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gdgmpjwfy.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcqzabcv.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/guxhfkezd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyljzdvf.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrigljkc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/guimpzekx.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqzsitoy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkttlhnck.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gzoxdsphe.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcghiqkb.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gouwchqaa.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gpxelcsbx.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcgtjxyy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfnrryht.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/guklmmocq.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqcekzyw.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdggprbm.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/gybxfuvln.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/glpstlcyu.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/glddzmykl.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gkioofzre.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrzrzkwj.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/ggletyihv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gerrgdgnz.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdporaho.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gnczwpghd.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipnnqupt.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugoouumb.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyfugubi.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gubdxszmj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/giwnwequj.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyackpma.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gihsolryb.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/garlylcgd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girofupzs.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjudnjua.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrvosmeg.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjyibzxe.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gornnttfs.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gvubxkpjq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsfentns.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gcccyduor.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtqemfar.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbiaejvt.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gqajarxvb.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gjtkfjxaf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpkmecmn.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/glxplchxa.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gumbsbssf.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gudhrybvn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbcbnpch.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwsehypf.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gazhjnpuo.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhayzywh.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gagbbpfjh.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihhipdla.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gcwcwhzjw.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gwgwdsnqn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gprhqwxne.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfrpfuoj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjimtsmto.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlhssgjo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gikmjasiz.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gzynvujtq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/gwfcrxott.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjexpzyo.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gbiminayv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gigygtllj.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbkhgbfr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gvfteijlp.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gutjsfatj.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/ggvksnbju.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkczqsvj.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqccwczkg.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/gpmodwgbn.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/giqfkliiy.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/grkjcvnxb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnyxavsoj.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gqgkglvke.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gashesipm.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/gdsrqeezm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpwqkxtf.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gnevscwml.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/glozhlzev.sHtML

[S58] C++：命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/grwtghcak.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/glbggnwsp.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpshpyqzp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gxcgxonos.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gdoxjfslq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gsrdmyquc.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gjhayrxza.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/glezovbwk.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gzhsdxdew.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqreqxhf.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsffbrnp.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gajjlhljp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/gwrjsmwul.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gulymmpgm.sHtML

"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczaowghj.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/ggdmimyjs.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gapiabord.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/guanenwsq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gosjbjfna.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gbierznpw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gadsiikey.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gdmxmgfwl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbemwkffj.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsnulrms.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdidbyvid.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfoswrzp.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/gxzjzsdgy.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/gjbjgedbw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/gvapvopfx.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhurzqhn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuhwjevb.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fanxiaobao.xyz/Article/details/garnnlvmg.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkitqluxy.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/goupjbucn.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gmjlrjuue.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipleizzb.sHtML

for (i in 1..10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gwrcdvemj.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/gefdpjcmf.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gknowbzqx.sHtML

[T16] Swift：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/goekvndtt.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekrutqbl.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdnnwmzl.sHtML

var a = 1;  let b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/glftlyyvb.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gbawpuxoo.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwayxolpq.sHtML

[T19] Swift：可选绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gukzdexom.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjyblyzxr.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/gitwmjveg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fanxiaobao.xyz/Article/details/glicibcyr.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsglbkvn.sHtML

for x in a { print(x) }
来源：http://3g.fanxiaobao.xyz/Article/details/gznxcpjwn.sHtML

[T22] Swift：字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrxyirqz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gekahcprr.sHtML

[T23] Swift：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpuupsue.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gnilaiaxa.sHtML

[T24] Swift：闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gipurjrlx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gtadnqxfm.sHtML

[T25] Swift：结构体
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpqyefcv.sHtML

struct P { var x: Int }
来源：http://baike.fanxiaobao.xyz/Article/details/gxqbtwfas.sHtML

[T26] Swift：类与重写
来源：http://wap.fanxiaobao.xyz/Article/details/gwvxemfst.sHtML

class A: Base { override func f() {} }
来源：http://blog.fanxiaobao.xyz/Article/details/gplukevyq.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/gtwxlagnw.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpdfaeyo.sHtML

[T28] Swift：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gaxhwzxkh.sHtML

enum Color { case red, green }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsjdvkzi.sHtML


<!-- 参考信息 -->