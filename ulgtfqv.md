代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/gyjhpnvcd.sHtML

[R18] 遍历数组
来源：http://3g.zdbjq.cn/Article/details/gjzxsahxo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/gbzpnmnko.sHtML

[R19] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gsyudpqfn.sHtML

echo "${#arr[@]}"
来源：http://www.share.zdbjq.cn/Article/details/gtdobxkoq.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/gagsxlrsf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.hesvh.cn/Article/details/gpedkejke.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/gftqvkutq.sHtML

echo "${#s}"
来源：http://www.m.share.zdbjq.cn/Article/details/gsvqnugob.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gvpbzkrsw.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/gmgbikqvw.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gpdidbypr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/gbrvnphwy.sHtML

[R24] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gswqcjtfy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fehbvm.com/Article/details/gwnebpsms.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/godapbkus.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/gnmhpevyx.sHtML

[R26] 命令替换
来源：http://read.share.hesvh.cn/Article/details/gwuazdjmx.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/gizoddcwv.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/giphjstnp.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fehbvm.com/Article/details/gvdrugxlp.sHtML

[R28] 浮点运算
来源：http://wap.fehbvm.com/Article/details/guglzoidq.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.hesvh.cn/Article/details/gstxclkqe.sHtML

[R29] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gbfhofpml.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/gpahtwxtz.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gqqwuylcf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gjnskekjt.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/ggnquouso.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.hesvh.cn/Article/details/gegsivkbb.sHtML

[R32] 参数个数校验
来源：http://blog.zdbjq.cn/Article/details/gmcpdjohb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/glzpnnyyv.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/gpbscktqk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.hesvh.cn/Article/details/gsduhiycg.sHtML

[R34] 退出时清理
来源：http://www.blog.fehbvm.com/Article/details/gotwosstj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gueqicedz.sHtML

[R35] 后台执行并等待
来源：http://3g.hesvh.cn/Article/details/gbtnveucd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.zdbjq.cn/Article/details/ghffnrpnu.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/gumbjlqpv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fehbvm.com/Article/details/gmuuabskw.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.hesvh.cn/Article/details/gseufnzfy.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/gqvwobsac.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/gqdwswzgn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.zdbjq.cn/Article/details/gqyekmoud.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.hesvh.cn/Article/details/gamxitklm.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gqwykatst.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/gjnxysnge.sHtML

echo "log" >> out.log
来源：http://blog.zdbjq.cn/Article/details/gexucunah.sHtML

[R41] 丢弃输出
来源：http://www.blog.hesvh.cn/Article/details/gpqedzech.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/goumdntdf.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/gkpvoqhcw.sHtML

wc -l < a.txt
来源：http://baike.fehbvm.com/Article/details/gzcyyaaai.sHtML

[R43] 按名字查找文件
来源：http://www.share.hesvh.cn/Article/details/gdiruvfxw.sHtML

find . -name "*.log" -type f
来源：http://read.share.fehbvm.com/Article/details/gpiuskjds.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fehbvm.com/Article/details/glzrdvpli.sHtML

find . -mtime -7 -type f
来源：http://m.share.fehbvm.com/Article/details/gphmdlvmm.sHtML

[R45] 批量删除
来源：http://baike.hesvh.cn/Article/details/gkrlvzhof.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.hesvh.cn/Article/details/gtksxztpi.sHtML

[R46] 递归替换文件内容
来源：http://m.share.hesvh.cn/Article/details/gqmyglrhl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.zdbjq.cn/Article/details/gcfoxatcz.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/gjsbocrfn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gttngogim.sHtML

[R48] awk 取指定列
来源：http://www.blog.zdbjq.cn/Article/details/gbrrbaupu.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gkdifexaq.sHtML

[R49] awk 带条件
来源：http://www.blog.zdbjq.cn/Article/details/gmszrznfv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.hesvh.cn/Article/details/gyrnyfwbg.sHtML

[R50] awk 求和
来源：http://3g.hesvh.cn/Article/details/gvnfynmzg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gaqnpfyrl.sHtML

[R51] 排序去重取前几
来源：http://m.share.zdbjq.cn/Article/details/gysxlpcht.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gbyrkdmwy.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/gyfadjtbe.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/glfoloqaw.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fehbvm.com/Article/details/gwvylqboi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/gcziaetsa.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/gpjxxhnvt.sHtML

diff a.txt b.txt
来源：http://baike.fehbvm.com/Article/details/grgpvwmuk.sHtML

[R55] 压缩与解压
来源：http://baike.hesvh.cn/Article/details/gexhwdvos.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.zdbjq.cn/Article/details/gxbaiagwf.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/grpbkbfse.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/gsmylvkab.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/gxkwunkdq.sHtML

ssh user@host 'uptime'
来源：http://read.share.fehbvm.com/Article/details/gnmpbgjhr.sHtML

[R58] 下载文件
来源：http://m.share.fehbvm.com/Article/details/gltalitzb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gvvzjjpwe.sHtML

[R59] 发 POST JSON
来源：http://blog.hesvh.cn/Article/details/gjsorqvhx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.hesvh.cn/Article/details/gwrictgno.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gutjrslqt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.hesvh.cn/Article/details/gbqkejtil.sHtML

[R61] 磁盘占用
来源：http://m.share.fehbvm.com/Article/details/gqvpyhocw.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/gfywmifkr.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fehbvm.com/Article/details/gudmcarqk.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/gjvdrdbmm.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/gzyhtpdii.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/gjsiaemvz.sHtML

[R64] 结束进程
来源：http://www.m.share.zdbjq.cn/Article/details/guaboplbc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/ghxkciuqe.sHtML

[R65] 查看端口占用
来源：http://mobile.zdbjq.cn/Article/details/gqarzswoe.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/gxadukdyp.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/gzjotozfy.sHtML

crontab -e;  crontab -l
来源：http://wap.zdbjq.cn/Article/details/gdqmmuekp.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/ghekxgawy.sHtML

openssl rand -hex 16
来源：http://www.blog.hesvh.cn/Article/details/gniorpequ.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/grwwcffhv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.hesvh.cn/Article/details/gqwdqfepg.sHtML

[R69] 生成随机密码
来源：http://www.blog.hesvh.cn/Article/details/gxxscbwza.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fehbvm.com/Article/details/gmbsduvoo.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/gxnrgcxwf.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.zdbjq.cn/Article/details/gtoxstpwu.sHtML

[R71] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gtowubcnr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gsabqvjfg.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/gkfyeqsrz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/galioweec.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/graqjgtqk.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/gqreskxvl.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/gaocwcahk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.zdbjq.cn/Article/details/glgpedlnn.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/gwyvxlhtt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.hesvh.cn/Article/details/gzwpogmif.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/gyxwjehkl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gkvrjugda.sHtML

[R77] 读取用户输入
来源：http://baike.zdbjq.cn/Article/details/glbyjjjpm.sHtML

read -rp "请输入: " ans
来源：http://m.share.fehbvm.com/Article/details/gypswbsyj.sHtML

[R78] 交互式菜单
来源：http://blog.zdbjq.cn/Article/details/gbbahbqii.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.zdbjq.cn/Article/details/gkeppqwzx.sHtML

[R79] 解析命令行选项
来源：http://wap.fehbvm.com/Article/details/gyzdopudi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fehbvm.com/Article/details/gwkmznejc.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/glkigehqk.sHtML

time ./run.sh
来源：http://www.m.share.hesvh.cn/Article/details/gqrawwatz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grfponwdg.sHtML

S. C / C++ 专题
来源：http://baike.fehbvm.com/Article/details/gfavabkyz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gnowgwtit.sHtML

[S01] C：Hello World
来源：http://blog.zdbjq.cn/Article/details/gqurctlod.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/gffwlenxu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fehbvm.com/Article/details/gwrfwmmjf.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.hesvh.cn/Article/details/gqsrejlam.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.hesvh.cn/Article/details/gyxuuywyd.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/gcvehotht.sHtML

int x; scanf("%d", &x);
来源：http://blog.fehbvm.com/Article/details/gtioblhxa.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/gjlxhqnhd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fehbvm.com/Article/details/guusgikjb.sHtML

[S05] C：字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/ghmxqyszh.sHtML

strlen(s)
来源：http://read.share.zdbjq.cn/Article/details/gnzfrsrqd.sHtML

[S06] C：字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gdqewhujy.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/gefdqcxro.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/gcprldjav.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/gzoapjjyn.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/gkoqkljtl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/gfdnftscb.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/glbarvkkb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fehbvm.com/Article/details/gyauuqnzm.sHtML

[S10] C：指针与解引用
来源：http://www.blog.zdbjq.cn/Article/details/gfcppswys.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/ggbozwflk.sHtML

[S11] C：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gnqxrxcnw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/gdprudmqf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gajtdvjwb.sHtML

fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gaysnupiw.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/ghuhjrzsl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fehbvm.com/Article/details/ghkqytrly.sHtML

[S13] C：宏定义
来源：http://baike.fehbvm.com/Article/details/gdyauuifl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/goggglxvc.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/ghssggxyp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/gbvfqmoxy.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/gqvrkxxuj.sHtML

(double) a / b
来源：http://read.share.hesvh.cn/Article/details/ghfwirzbc.sHtML

[S16] C：位操作置位
来源：http://baike.hesvh.cn/Article/details/gteqdvokh.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gjszldzxm.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gfceknmsw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/gugdrieim.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/gwkoogvfs.sHtML

int main(int argc, char **argv)
来源：http://blog.fehbvm.com/Article/details/gpxwiyeul.sHtML

[S19] C：快速排序
来源：http://blog.zdbjq.cn/Article/details/gwtolmgry.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gycrmgazt.sHtML

[S20] C：二分查找
来源：http://blog.zdbjq.cn/Article/details/gqhdspyfd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gdfzbsmsg.sHtML

[S21] C：字符类别判断
来源：http://mobile.fehbvm.com/Article/details/ghnxplthr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/gvgdpzckx.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/grlfommuf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/grpitfqjd.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/gmetrzfge.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/gjzuyfndj.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/gbydmpyzd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.hesvh.cn/Article/details/gfypztrco.sHtML

[S25] C：内存拷贝
来源：http://read.share.fehbvm.com/Article/details/gzhokabls.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/ghhbnbpwv.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/gpepizpns.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gntpvqbfq.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/guwccxabz.sHtML

const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/ghtlovgxi.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/gjzwcxegt.sHtML

static int counter = 0;
来源：http://3g.fehbvm.com/Article/details/gioyhmnax.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/gahgopmkv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/gplnodxgc.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/gymvliaql.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/gsbwoorto.sHtML

#define X_H
来源：http://www.share.zdbjq.cn/Article/details/gjmfzplus.sHtML

#endif
来源：http://www.blog.fehbvm.com/Article/details/gdsyrsuii.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/gjgqckslk.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/gatybenyv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.hesvh.cn/Article/details/gtsazmiap.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/gdgagleng.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/gpxakikpw.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/ggjqoihid.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/gzwsaeoxn.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/gdiidhhmn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.zdbjq.cn/Article/details/gztbwvwco.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gksglfqxd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gxwnahrio.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/gpbylwynq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gwpripcjf.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/gfhqixsux.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fehbvm.com/Article/details/glfvqromn.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/gyswqhsex.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/gxqybkjac.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/gyneztekd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fehbvm.com/Article/details/gvqbgkuvl.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/geygleara.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/gdqhscpji.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/gzbfexudk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/gkscadmjr.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.zdbjq.cn/Article/details/gtzqflsqy.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/ghgukgqkv.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gwaeitqfv.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fehbvm.com/Article/details/gdnjcslip.sHtML

[S44] C++：引用传参
来源：http://blog.hesvh.cn/Article/details/gkumllnsx.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/gmoazymtr.sHtML

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/ghxideweu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.zdbjq.cn/Article/details/gyuqmsryn.sHtML

[S46] C++：函数模板
来源：http://wap.fehbvm.com/Article/details/gwnrxzkpv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdsarxxro.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.hesvh.cn/Article/details/giezmfiez.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/gvguwxdtx.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gqybfeggo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fehbvm.com/Article/details/gnvsyncco.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gjqptsttm.sHtML

[S49] C++：写文件
来源：http://wap.fehbvm.com/Article/details/gqigzmxyr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/gliytthtr.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fehbvm.com/Article/details/gqmuhwghp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/gmkdrezee.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/gqyyfdqov.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/guldbkakl.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gpjhvensz.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.hesvh.cn/Article/details/gxnjnkzpn.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/gbxqyuxoc.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/grtjtrvws.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fehbvm.com/Article/details/gttmhsmrk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fehbvm.com/Article/details/gufvnhikw.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gsvdhiepz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gqngbpsxd.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/gsislnevv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.zdbjq.cn/Article/details/gllyxorvp.sHtML

[S57] C++：编译期常量
来源：http://baike.zdbjq.cn/Article/details/gazfndfxj.sHtML

constexpr int N = 10;
来源：http://3g.zdbjq.cn/Article/details/grbllmmlc.sHtML

[S58] C++：命名空间
来源：http://www.share.fehbvm.com/Article/details/gjosoaxwk.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/gxknrstbx.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/ghxbixnfq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/gaxutqaqv.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/gjzrltlpf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.hesvh.cn/Article/details/gznvabcpe.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/geaheeiax.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gbfxuaylo.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gaofrdaod.sHtML

[T01] Kotlin：Hello World
来源：http://wap.hesvh.cn/Article/details/gaajxvieo.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gzckbogqx.sHtML

[T02] Kotlin：变量
来源：http://read.share.hesvh.cn/Article/details/gblpfvgun.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.hesvh.cn/Article/details/gcqkqghet.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/gdyabpbfj.sHtML

"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gwsroqgfh.sHtML

[T04] Kotlin：空安全
来源：http://read.share.hesvh.cn/Article/details/gkcpydodt.sHtML

val n: String? = null;  n?.length
来源：http://m.share.hesvh.cn/Article/details/gnagbrqdf.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fehbvm.com/Article/details/gulezyogh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.zdbjq.cn/Article/details/gsmcpdxfd.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/grunpbcvd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/gtqdbkqnh.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fehbvm.com/Article/details/gqjfzzoky.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gzcfubvrw.sHtML

[T08] Kotlin：数据类
来源：http://blog.hesvh.cn/Article/details/glkgzqhbs.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fehbvm.com/Article/details/gdvymcopk.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fehbvm.com/Article/details/gsofigijx.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.hesvh.cn/Article/details/gkkjuuhsj.sHtML

[T10] Kotlin：默认参数
来源：http://baike.zdbjq.cn/Article/details/goqhfqsue.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/gbiifsqbv.sHtML

[T11] Kotlin：协程
来源：http://m.share.hesvh.cn/Article/details/gnjtizzvp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/gxeqklyon.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.zdbjq.cn/Article/details/gwifescsz.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.hesvh.cn/Article/details/guloxogqn.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.zdbjq.cn/Article/details/ghlwwmwnu.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.hesvh.cn/Article/details/gmdxmsdoo.sHtML

[T14] Kotlin：循环
来源：http://wap.fehbvm.com/Article/details/gmgsjjnay.sHtML

for (i in 1..10) println(i)
来源：http://baike.hesvh.cn/Article/details/gwkkpdckh.sHtML

[T15] Kotlin：接口
来源：http://www.share.zdbjq.cn/Article/details/ghxthyuou.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/gdknakztx.sHtML

[T16] Swift：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gwtxghqoj.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gsgvnuxec.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fehbvm.com/Article/details/ggxccwflt.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gowxbhiye.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gefzdvbot.sHtML

"值: \(b)"
来源：http://3g.zdbjq.cn/Article/details/gfoykunga.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/gqkpznlzd.sHtML

if let n = opt { print(n) }
来源：http://wap.fehbvm.com/Article/details/gogqglnrx.sHtML

[T20] Swift：数组操作
来源：http://mobile.fehbvm.com/Article/details/gnubyfajp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/gbnhazdcd.sHtML


<!-- 参考信息 -->