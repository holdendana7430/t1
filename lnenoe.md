代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tdcbwjkk.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3nbxkvevv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ajrfkgmm.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3qzuwhbcm.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3utfcwzpf.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3cngqiflz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3avuwvnji.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3bsrflanq.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3ffqhpxmy.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3xmwwkdvu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3qwyaqgbi.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3xzshxyzv.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3gpigrucl.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3nsihgdps.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3fmludcnf.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3epwrihdl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3vydkwbed.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ouipayva.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3rssoiokm.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3ktqdvlee.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3glzyttse.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3fodtguqt.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3plrfwaar.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3klmaxjmu.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3wttblokf.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3tjdwdzez.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3jzohbqhr.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3qbzzhvba.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3mfpjzyuz.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3lbnvzxqe.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3voltcpga.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3linguvqs.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wgwhvcdi.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3dlvzqarf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ppnfoqgg.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3xbhzpqys.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3audrivnd.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3avvlwjna.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3xmvjwwdb.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3rprcvbyb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3eechjhaw.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3lopljkmp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3kjvceret.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3pnozzjph.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3iqjetxkq.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3nbsdqhhl.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3heqlyxnx.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3tszlvmch.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3nmteuuiv.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3lzlpbrsn.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3twqmzeyc.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3mtmraitd.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3gnjpehzd.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3bzdlwqhh.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3xldvecdr.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3yblkqyvb.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3vqlkndbh.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3hjbdojcf.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3ftcummtx.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3foyckoci.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3zpcajjsz.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3ektsumei.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3oczjgewd.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3uuioxrdl.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3bvpiulyb.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3wisjhcpg.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3swcfrphd.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3rzyhgkns.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3bkowhinn.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3vtlsrrhi.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cgubfomq.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3mbuscokh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3onbgjatu.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3wpmwdjts.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3jyabcnjf.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3gtsypmnt.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3fbonrhkd.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3adktpcvq.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vqqdmiyx.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3ziaqirah.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3akmxorxo.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3okonmgyx.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3ddltqzpg.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3irjwdotz.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3eiatecxd.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3zroqpvap.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3txbjyqaz.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zijdrefc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3xgncsoav.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3urhkpnlx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3nxeihldt.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3hjpmbexi.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3gfsnipao.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3mqwlhqve.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3jhfrkloa.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3fypryfpf.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3twufgyee.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3jstzngbq.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3ligwuein.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3jhnoqngu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3yzkbdwdr.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3sgnpyqwn.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3jkrdmkeh.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3qhdhyisk.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3jhdeuwbq.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3sdukteib.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3abuvnbxg.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3lyajoapd.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3rmdjmpgz.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3psklznnq.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3oodfzius.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mrsumjly.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3yqagamql.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3lfcjegod.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3onrkghdk.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3ccasrzlu.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3ioqobfwo.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3ijprrelc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3gkqgioek.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3kdkagmnh.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3mnsroczw.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3wzkpkkbx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3rcwhgqzg.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3kbwoazzw.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3jrusfwki.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3atxbichh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3vmoprvmd.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3ltfusiru.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3jigjudpi.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3ahbeyleq.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3nenwtasm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kmvgzbti.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3mmlwhhwv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vhltyoon.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wfbiisfi.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3xrijilry.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3ruttewrr.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3sbzfbwty.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3fmrtufgq.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3wezijtov.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3mdsrxlsc.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3anqtspxk.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3owxiuzta.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3xbktligs.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3smnmrktk.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3xjwoiyht.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3ymtedeut.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3khbqptki.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3tzyeubbx.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3xbdmjkai.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3ddpcwwap.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3lsjidupu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3cvvwbfob.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3urahzjsi.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3mfqttqru.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vybrccau.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3rukumakm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3jksdbzvt.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3nwuintbn.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3msqcvyvy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3jkgxnzzr.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3gdqtcqtd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3qbpztlkx.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3sswcejht.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3njpkifus.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3bbzzemvw.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3zrwdfiut.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3llmzaumn.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3dhkpbcli.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3eszqifze.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3abyzutlq.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3eazvszpv.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3gtrartpa.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3oquxhurh.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3sksjklln.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3bzlzkrph.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3grcsbqty.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3qckdhmyt.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3nmgwdtux.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3bknyhwdu.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3jwdazjxa.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3wgghuove.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3rtkzjgan.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3bdiwxmwx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3xfmymuho.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3gbqpnuqj.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3vejfwzts.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3plkdrziq.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3zusmrvhr.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3uqotjlry.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ayiokzrp.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3zikbysla.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3zdlzlsdu.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3ucyvbnkl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3upphtaqg.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3egolvwra.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3zpegjbfj.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3ixfkzxsu.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3dxhydded.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nqiggmys.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3fgayrtnk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3netebuvz.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ylrskfww.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3treltcot.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3xsbgqmtu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3gaqedraz.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3qooukixn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3caktxwqd.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3mfcbkkbr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3smqicwth.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3xztoliyu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xfmvgagz.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3sfjkubwc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3sgyhhikx.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3wcogmouf.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3jvuosnad.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3kelfjddv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3qdykdizq.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3bzlqyyee.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3twhqtief.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3nvulwadk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3xanndziv.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3lsiynnnj.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3kenetpxu.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3tkldwirc.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3runvfrlo.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3rchfetrn.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3bisuwmuq.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3igovfjrs.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3atjpqsdg.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3ahvrmqgo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3arjjewbd.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mqhngxfj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3whddsrnd.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3qwjkuaky.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ktxmnywy.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3elvakotu.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3zoggmiaz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3btfzdqke.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3zeglezzp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3iluzjzgy.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3tofjrpom.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3loouohnp.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3lvyoiwxc.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3acgxyzfi.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3kxvklqjl.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3oswrvbnl.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3ykglciig.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3wqxvzmxr.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3xgknaeop.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3rxjqyslz.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3apfumaml.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3vtrihkzd.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3cazekann.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3klzepsjy.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3vlqkglxi.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3rjjyxbtr.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3rzjmaqlw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3lnxmfixs.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3iccbermt.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3kraubmip.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3btcgkqhe.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3gztdipbb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vuixryhg.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3buvpojth.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vkkskujv.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3pbttqsez.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3wuqzsbcu.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3ywgrbcjw.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3kbpjivmb.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3efvpccao.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3opvbvawv.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3ixcqzodq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3efbnhxzz.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3sdjaqoza.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3rvbbcxck.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lggtfiqe.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3tvptzzek.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3kgmdluge.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ohtqxhai.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3ovnermac.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3ybwzqtpl.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3lkwcawje.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3vqlxxhvd.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3azuypmex.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3ydnvgtvm.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3fnkzszdy.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jvxcdiii.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3xnfnkmcj.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qkstaxks.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3racgzsnw.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ofeaihnz.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3pjcpnrrz.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3tgmnaffu.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lvomszsf.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3byikhltv.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3pdtgtcnl.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3kfgwhgku.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3knmudykj.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3totifqfm.html


<!-- 参考信息 -->