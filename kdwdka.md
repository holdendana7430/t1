代发 wailian999

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3npfrazjf.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3mrfhvlps.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3kdakykle.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3igjbaqiw.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3hnureajl.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3idqldent.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3pjtthmaf.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3xygnxeyp.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wpejrwxv.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3qpfdrrdo.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3gseqaxyd.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ugdvvlcl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vfovxftx.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3tlmdqtih.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ulqsiqhm.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3iqsvyfqy.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ylrwrkyb.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3eiegepzq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3frpvrxif.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3jksmytst.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3qwheiual.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3wupbrsxo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3vapjxcqf.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ueazeiub.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3lvuvrizn.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3gdagwkse.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3kdzowwta.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3xlckviyf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3jdeyqsmp.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3akpiezns.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3wisscrde.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3mtwnrzet.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3nnbtapia.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3yzvjxkjs.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3nbtsrrca.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3ubirzcae.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ytnffiib.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3baqsumpo.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3rknbjdqd.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3eplidjxx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3ialyjuge.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3thkihbbs.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3eufvrhak.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3iiuoupjx.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3xsubpkvv.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3ojurdxjm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3hsdxsemm.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3daciiybv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3zjvsmnvo.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3fpvjetav.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3tbbofdbu.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ylkrdxjm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3shobcjwp.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3fjngbwxh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3khfjjrnl.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3ekydlsbl.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3pkdkpqhx.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3dwdzcahv.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3zxrsujbv.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3tifpypse.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3xkdxitpr.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3quswtton.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3ztrqhubz.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3wpgdctpq.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3prmoxndp.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3penccfvg.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ppvtalvv.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3vfrgihna.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3atepfrjr.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3emfkwgrp.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3anvkueuj.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3facsonaw.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3cetsboqk.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3booaeawg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3kjoerekw.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3vhbvzxqk.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3glrdeatr.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3szenhnml.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xgshlfdu.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3syaoabya.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3izcmlmvw.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3fmhwghzi.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uiksqvfk.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3luphkcwo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3pimqppjo.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3atwqxyvs.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3quykkvgu.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3zoekfazw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3ewmeioev.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3hwqiqhhn.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mippuhav.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3qflfqwve.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3nuoshhlb.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3hlrjymwc.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3pvofuzvo.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ktdcfhuw.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3papsabhd.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3tarnjkie.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3vofxcwog.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3wfsidbsp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3feaxfqbt.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3lrrueqeq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3tuooexag.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3qseumnsu.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3lncqrpqy.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3qzngspjl.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3ihnwkyoa.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3qrklgtjg.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3ylbyzuri.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3fzsmnjgc.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3ngygqgna.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3glgweyjh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3eixwnxam.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3mitcnqam.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3mlxbykdk.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3xzcldohr.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3dvzvbgfl.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3wbwmaipl.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3voentbvo.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3pjinkasy.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3vbuggyql.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3eknmxxcm.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3gxusoebo.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3hohqerua.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3quqmtydu.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3sjniivcg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3zlhpbpmr.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3dxsciblf.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3zwyujjzv.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3hxstojjz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3lzzmmoiw.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3qketcbvg.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3aykkvctg.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3ypyvjitw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3mwkbatey.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3przzlpbj.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3buiinhsm.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3rrjnjxec.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3hcldgijb.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3ypmjrlog.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3uqheteqj.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3bblzcjnn.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3irqmprvd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3muokauez.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3gxgwwxaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rvxnslxp.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lpwbppbb.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3occqblmg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3zpgvecza.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3txrcjvvs.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3dugzmuxi.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3tnttnbwg.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3jjnyfazg.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3pwgqgqmq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3cbuoyfim.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3srmllhfe.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3gwhbolmf.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3wcjkevsv.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3vrrmaxdg.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3ymjyehty.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3ufcjyhnp.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3qoyszzmd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3lnpfzppi.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3elgvlrxd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3nwamejsi.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3ubraxsmj.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3pihxcmjn.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3emsrlyon.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3dahmqqge.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3qiffgamd.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3iqmaaepo.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3hjwcgyim.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3leegybso.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3kcsewqrw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3pprlifcb.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3cpdcnzvo.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3flcsusus.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3pfixmmrh.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3czramyzp.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3zzugdvsk.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wlqdgenp.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rlqgbciv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3kydoyqte.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3vqpdqzdm.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3saklwxzt.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3iijlrhmg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ognrkynn.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3hqwxumlu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3lexafjdk.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3ihmjsbzu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3ujjpsqiv.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3cngbpdbz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3lgssfwqu.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3hkvyelfu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3mtfszxtk.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3yxhehmpc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3teghuixy.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3wetcsgam.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3wkvhsvsa.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3vgqfdidv.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3mvxvihva.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3cxdpvalv.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rdrvxzks.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3aaljyeib.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3tlvpzgmm.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3xvlzggfz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3isjrztdz.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3bklyesob.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3spzhllhx.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3oppcydvv.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3ijqujiod.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xtklyyud.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3ebeazsbp.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bllnzxoe.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jjenowwa.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3gdjsxsfr.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3euufihgm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3lsqjwhum.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3mvmjxujr.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3oenhtfoi.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3xbqeubgn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lmbmdcon.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3jydxcoin.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3lhtxlmme.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3tcvtthgf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vedslxwp.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3qwgbhswm.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3fgkqvonp.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3cfcvbksf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3jsqrwvsi.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3vbynaogl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3oluaidcy.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3skbjtfrf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3hqseodup.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3lyywxsqs.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3rwrhbbdv.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ejiswaya.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3qdjozewu.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3kuvbqvid.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3aibopfzg.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3phkohrgr.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3upwzsnwo.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3bzudgqfp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sabacezo.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3myogothi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3cgodqpwy.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3abzswzja.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3upqsxilk.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3eisgmmiw.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3cvexvoqu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3qxljowgc.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3ybwlkiam.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gwjwqfid.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3stdeepyk.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3ciqytbvp.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3pskclrej.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3sysyfwvo.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3yzxhgkqs.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3bwxpdntq.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3fpmkmoga.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3wczygeuv.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3gxojnerz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3fxcggckl.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3yxqouksg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3ryncwmha.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3qzzkpynv.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3gbizsidh.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3nclarcxf.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xwoervxg.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3kghixrrr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3beegjtzj.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3msycwttw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3aexeevii.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tawuesjg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3aikalhzi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wqkcghuq.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hijvbsdr.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mtzapyaz.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3dandljuz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3oeaxmqpy.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3ltmqefjb.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3jmqugkqw.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3fkctwlif.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3mzlospbc.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3ayyviqnx.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3jgkjuuvo.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3fhiqxezu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qkcnlkjz.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3tbldzirr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3zsfpdjvm.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3iqfosnca.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3xltiescy.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3swlrcydq.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3eqtqprec.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3gpksylqj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3kpuvfgfy.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3kdvewpfo.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3apwtbnnb.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3ilvumhkp.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jbjfhpfh.html


<!-- 参考信息 -->