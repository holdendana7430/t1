代发 wailian999

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3djjvvqaj.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3cnbzixmo.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3zfznfjuy.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3nefkbzly.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3kczatqnm.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3esnctojt.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3zougjpow.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3dsxlcbtg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vloiyxeq.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3ajgprfpv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3fhwnfyqk.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3pwkbuupf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3cwlpblrm.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3lidvvcrn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3fbhobzzt.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3qggcfxmi.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ifiqjzxd.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3cakgeplr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3unkizdga.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3vnozpgpu.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3dfjufxmg.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3xtdwiaqt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3cyefkppa.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3trypjmhh.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3vshgwuko.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3aifzrmob.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3yhpytptx.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3iyyppdog.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3bcnxnywa.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3chbuagqv.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3jxeybftb.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3nynutjtm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3voygniba.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3fqfdwlwv.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3lbteejzy.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3npaoouza.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3buwhclua.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3nummszcm.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3bmujcxpw.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ggyoejqa.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3cmeihpmw.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3rwboshjq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3jqsddpkd.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3skurdiqz.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwikxtcz.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3gynisosw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3eiksalqx.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3ghienslg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3hpguepjz.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3mqgzryls.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3adgjmpfq.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3vgtutxsm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3eboanubc.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3rdicyqvp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3tyqprjox.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3pkiqfikr.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3wyetjbau.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3zmvafosr.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3atsoffbe.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3wgewwwxd.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3umnmkykb.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3nsyqxjgg.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3qphpogxt.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3ztzqwqej.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3cxbuusgv.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3zxpcwrmj.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hebcnmgu.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3hznvscsu.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3omdpscob.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3vpppfjqd.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3avzhirsx.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3lctcywcu.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3ywhcnrug.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3qvbyynsz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3xhiepltq.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3coswiedc.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xdckhbhs.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3rjuyjzru.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3fhlnfbgh.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3khonwzed.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3jmnqeaet.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3nlzphlzo.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mojwpbud.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3cximjkpv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3utramckw.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3tcqttmgi.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vusbyqpn.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3cdvusfye.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3qdhtdtuf.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3pmaqfuqd.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3cczrptpe.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3xpodckcl.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3boqankaj.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3wqctmvnm.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3qtgjuddm.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3hfhrdntk.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3oxctxbfx.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3lgrteurh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3lprutila.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3jbxrlbjg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3bmdhexpg.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ujnnchpc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3phfcztky.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3ugkldiqe.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3aptwsrmz.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3hkoryzbq.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3vbahxmfs.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3ipakandj.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3sbowmsfb.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3aflayemo.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3inuhatoz.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3xtmsajcz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3yvjatwjv.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3cujwbryo.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3smlrlajr.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3cowglxzy.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3jiocaxjm.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3xyquiwqe.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rqljbeys.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3khqxdost.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3tyifqmcu.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3yxmkmzva.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3kyfjpjow.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3viomflpg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3nqpidjgg.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3waadzewb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3qbjwsqpe.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3mhayyxwv.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3lnnnjnwu.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3jubrxrob.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3ygivxrdm.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3wlrswuog.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3vekqbura.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3ihapumwz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3gypqjtgi.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3gcaibgtf.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3ckdebojw.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3desrrjex.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3hevyzyzu.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3pjwuensb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3kgffwybv.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3jsvhiyli.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3xlajysia.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ejvfyrin.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3tqkccrfz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iaiaqjgd.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3thdzyzfd.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3bxxjcikb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3yfaamoun.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3mvqchakz.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3wwmmfkkv.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3jkhhbkgw.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3trkxulit.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3rpfqgwwo.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3wbrclekm.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3wtdkiwud.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3ldusthpp.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3zahnohot.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3ocfgsunq.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3zqgmyisc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3bnkqhooi.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3isqiwmzz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3vkpdzicp.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3ibmciuhj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3ogjtgxbo.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3bdvrxbbx.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3kolhiqlo.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3pnqmehrf.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3onkmjrbu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3zwvmukdr.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3xjsvshis.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ymywwzzu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3gsijqttk.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3pbwrqdvy.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3cuslcqzc.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3lcbrbxrn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3pqqwhfco.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3qgnmflnx.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3tikcaosp.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3lbbiewmq.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nhnqqars.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hlxggtgo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3rkrfnefw.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3lhmdhrza.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3gwmtwxyi.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3uhlxyjwg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ijhbhzjm.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3tazdnjdn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3mdgewdff.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3gsltcrne.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3olvtayvo.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3xsrurkft.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3uykwpqdh.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3qjsrdacq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3uiafjceg.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3yhizpjeo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3zbrfxgta.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3kfneppzn.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3osibzuyd.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3ipkbmrki.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3xnyzpurm.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3urwhvsre.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3objieecz.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3eimijmjy.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3fwftxcci.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3kthpbpfb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3ahlvuuvc.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3ciwptfij.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3sqslrhar.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3mhxcktzt.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3cldwxugo.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3imjrqlxc.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3yotsciit.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3jtoqvxtu.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3erkpsjfs.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3ocrrbowr.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3qtfjpvdm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3hqhdhogy.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3bvcoalaf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3qjiglbcj.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3exfnoyyx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qdyebmnj.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3wcmudttn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3akcpgyjk.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3rtigezxz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3prpecnwn.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3hnqgvneh.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ywtaeryw.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3qeblhayd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3tpmglcdx.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3xrgumxrg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3eruubokh.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3ylphnxtg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3rffmmabf.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3iqmcjkpl.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3sdunswtd.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3ceqskvjf.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3wxklzduj.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3syuygiuy.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3jdkbehps.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3uvdthcrj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3yboeggcg.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3mrpgmemk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3bbqtklev.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3akkfhiwo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3euvwgkoq.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3anqjrcee.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3xqonkyok.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3ykflgujk.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3tpuzsgpv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3kjqtfmiq.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3wtbryrqy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3udtdrodc.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3gyqpjggf.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3tfobushz.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3vqxqmdoo.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3rquqizuy.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3dtwtecxq.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3xmzukksc.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3xokcvmln.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3iptsstnf.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3slvfsasg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wmdqhlxv.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3sutwckbz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3pzyhgvdb.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3jiukzmpu.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3marubmkm.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3ivzepvko.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3cmmozejm.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3zooicjgm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3lwodaysg.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3syqvufuh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3nfmlkwcq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kgzkacdq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3yhyfbili.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nsvblydr.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ywuamtsk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3dluvukdy.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3cwpeefcl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3btuhtvwd.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3ekmlkbzb.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3vumjdmbd.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3cimpgvpu.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3gabcsvrh.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3nxcitiaz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3jmirhrvg.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3iirbrfub.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3gwhysbxt.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wlipnvey.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3bdvpfyry.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3kheptsrz.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3wzemhhac.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3mmpevgna.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3cmckcykl.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3mrxtclvx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3jpczxcol.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3mzhzhfoj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3ielqwwoz.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3heblyspm.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3unmgzuqp.html


<!-- 参考信息 -->