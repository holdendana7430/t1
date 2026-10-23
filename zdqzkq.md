代发 wailian999

esac
来源：http://www.52xcode.cn/Article/details/gt3svfcvwvl.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3ndmvedse.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3atxviupl.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3mhhptdrt.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3lrilvwab.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3gfptbvmq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bileautf.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3slygbkjr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ewoehgas.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3wbolnuqw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3wfxpdqnr.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3hxszrumd.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ebwlzwdl.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3rrncjidt.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3eoomrbyi.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3hvrqhbiw.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3hophkczn.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3gcncqmhv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3bovdqvlt.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3iymyevwq.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3uvrjykeh.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3zfotktrh.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3llndcedj.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3xaxlhjbz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3yotjxolh.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3mqlgcftx.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3cmokpvlf.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3rvwfpiws.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3qodekuyj.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3vvyvgiqs.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3byzwvyrc.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3bjjlxjvo.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3wlgeekxp.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3pmvthqgc.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3vgqznqbe.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3czwdcuif.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3xgswxmmz.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3yngwyxkg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3kpwvzpuz.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3umjpqwpm.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3avkruxud.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3cxedydpq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3kbcohovm.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3tosxwrjm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3fxwlskkk.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3hxzijwyy.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3mgbqqvmw.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3gufnlyvn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3ncycntjb.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3tnlumbxn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3cedtscoa.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3xanrihwv.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3glfvwdsa.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3shlwtrsd.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3lhjerszq.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3ckpzewws.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3lfffdywa.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3pukpqfgq.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3vbnrpljn.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3ojkgwwqx.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3xygkcaxp.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3mcyacrgw.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3eimjxlge.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3ikmyijmh.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ispoqdnj.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3mbhbgjbb.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3uwnnmqij.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3kctdikkx.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3ybqgqnoq.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3abzpnkae.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3eybsibaa.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3uvcwucxr.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cgedyyop.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3ymybaput.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ltdsxdys.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3djmwdhgc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3vskcsyjn.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3ssflsjvc.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rwnfbqro.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3hcmhgpsj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3mfqzadgf.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3rnxpugow.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3alhsuzvu.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3bnpziemp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3yvkdakep.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3jcunvmcp.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uwnuyeik.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3gtywejof.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3nevtqcrg.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3yssraojs.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3lpbcpvia.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ectoypun.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3ghxustsg.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3ypzcfgue.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3qaonbfqe.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3xvzplgxe.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3icpcbyqk.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3orcyrlof.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3auynvjiu.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3dvsrohgg.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3avqcfthc.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3xgfjvfnw.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3rtfemgrg.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3eymgynpr.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3lurtmrsu.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3ymqaaitj.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3vpxrsmer.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3vmlmcvla.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3csxvyoya.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3eriixyoo.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3atyvmtvu.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3movuvodk.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3zfkiymrx.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3ttfvewmh.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mbkcnbdc.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3gmzwozlt.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3flhprlnr.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3jlxsoljx.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3qqwwrzxc.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3vaadmnaz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3mxpjpgcu.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3rugmlncq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3oicpeipb.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3lawjakbv.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3bpuhwqwz.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3liomegbe.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hpttxabe.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3phogohok.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3xmamedld.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3pejifnwg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3pfebenpi.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3czbzrkzo.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3neognzwz.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3fnuqlebe.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3vmavsxcc.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3bcccrwvs.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3wackwwxy.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3nzclhrct.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3xvxovlps.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xxgszyyl.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3pcoihdvr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gyofaltj.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3clryfyef.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3hpinbmzi.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3dakehiir.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ytbwxlap.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3oayvtqzx.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3lbtztlvl.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3wyoeivap.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3oxzzbldo.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3wmkzhfnv.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3eaeufslj.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cuifkdiu.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3rzaqfoeb.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3bsziqwno.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3fasrsgyw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3xsnwrepc.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3azzurymo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3ksmtfnoh.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3lxybdlcb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3fpcvcngo.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3wmpuzbfg.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3thfgoqmm.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jhjrfwaw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3xanmsvsh.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3ulliplij.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3yyniktuj.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ziffzqup.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3lqmjcusf.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3vcbdqllo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3tpdhrgko.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3dkujlfuu.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3gbafdtms.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3ujtwezee.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3jogfxdwi.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3ipoxvfkf.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3fvapmett.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3watcqepy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3iejvlrbm.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3yjoebzkm.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3ukpqjloi.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3tykpewpp.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ultmbezg.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3bozumcjx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3suablbmq.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3pkcztgmu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3wobdwhbw.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3yurgpygc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3puvxckfs.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3xgpqdwue.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3bijwcixn.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3belzjley.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3dzqvfebi.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3yxwyzkjy.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3fehvgjzs.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3sdountwe.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3vtkkxint.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3jtvgjegm.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nydjunrh.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3llqpljrm.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3bljcqabi.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3xnmndjzv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3adgjrmbn.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3bdamglis.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3vgakxkoz.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3qhyyybfg.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3wcxsmwuj.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3muzaxzsh.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3ahdfrcan.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3hwhrcdkl.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3ynevlmbc.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3fdalndqu.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3bkciducp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dobhhryk.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3iktmpwwn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3rswqhjww.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ikypnvrv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yxjrwpno.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3sehbbtjf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mnpuujzs.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3jwhlnbsi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lsgpuznc.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3fykuejed.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3adxomokf.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3dkerscyy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3uyczesgk.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3hosfosla.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qwgytuvn.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3cxqmbmud.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3zvbqtizb.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3spkiifln.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3dbsberoy.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3lnutpfbh.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3gvmbhuto.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3sdqlxple.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3veoyvdht.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ymypdfhm.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3wvtflklf.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3xncpkyty.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3gisrrjao.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xthflluq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3pgdagskj.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wgcbjzcy.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3uprtovcn.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3xxmulple.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3tjwflcbv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3izcivyrw.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3nbshqtqv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hekupmki.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3ntwfxuzb.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3nnsktsao.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3ysvtiems.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3yixoykwd.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3sfgbagxw.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3lzyzgxor.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3ckrrljke.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3bmtdkgjp.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3tetobnvr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3drgwaady.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3cpmajsmr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3tjcybuhg.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3roazmura.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3ixuclbux.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ctimhmkl.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rveerdqp.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3abjgnzrb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3ghqoqzrm.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3rctjkiug.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3mssqgsql.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yuorozbe.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3nqjiaxra.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yjoprkll.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pbmixnfz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hieintml.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3mjloueui.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3ewlomeju.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3oatsqcaj.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3zztixmjf.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3tfemmjzk.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3hduirdgo.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3qftqcqae.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3rcqnblyq.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3qozmoryy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3opheiznk.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rcshopep.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3utmvdnug.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3ljwnkcbn.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ozkjlvls.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3mygnygim.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3rntmhjut.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3fqlzicxx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3odvgaood.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3yuvwdwhw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3kqexslox.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3dwjlvrdl.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ematnqim.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3gwkoeqtw.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wncqpdus.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3qondgmnt.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3idscsdzc.html


<!-- 参考信息 -->