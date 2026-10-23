代发 wailian999

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3rwkazwww.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3bhmmjsbi.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3tdyfkbdi.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3rdhinyew.html

esac
来源：http://www.52xcode.cn/Article/details/gt3dhtyemig.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3pbmekpyj.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3jqiauiaq.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3zrwwknsi.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dqtsjlqx.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3gyrwvphd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bvhdltdh.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3gkbgbgyb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3ezfalaxj.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3dctxhurh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ojbklvqs.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3noltuodj.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3dyadltzr.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3micmyegt.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ichvtewx.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3amacamzx.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3jlgnyaxx.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3ccwzifia.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3nnsakpra.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3zjlberho.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3lxhwvwlz.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3wjeyrdgz.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3bdcfgfqy.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3nwnemjal.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3rzjpjqkg.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3wylylhlq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3pdfbswxy.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3okwjuwak.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3mphrwsem.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3qjmzlbxr.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3dqzynstn.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3wdqveaca.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3zumzdppu.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3fpxmulqs.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3xhztdlfm.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3gfyrraog.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3ppiceozu.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3honsbwyy.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3cawlrprh.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ohbdfjen.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3hlvtyhod.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3uizexark.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3aecmdpoo.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3qecaffno.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3vqpojdos.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3eadzuuma.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3yspowjlh.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3xknviizv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3yqwbpmpn.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3ytfrucuu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3alxwstvn.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3siqgcvlu.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3tdedhwuq.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3sswwtuhk.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3dafvcvuq.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3djxlagey.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3xwmosigp.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3vxylosdv.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3bqacwnez.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3utybznka.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3pzyjwuku.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3eyglsvri.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3ctrepnup.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3ygdkqyzs.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3kqlofndk.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3tbnrnpdq.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3nueiaafm.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3euawyawc.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3raokuqvd.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3bvonomym.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3ljgalefa.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3uvxmneyq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3hzleyoho.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3yizldloj.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3srjudoqe.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3yoaovxzs.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3kaslpcyj.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3vtdlgndm.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3efonyuwr.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3pulueuci.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3mrhvljqs.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3frathyzv.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cnsrvnsp.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3qcelvsln.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3nwpagsha.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3vsjmbxmg.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3djoynpzp.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3kshqgoed.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3elucabjs.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3hhunqdrx.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3wezznwsx.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3dkyihfdp.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3rzzlvcou.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3dmwvwzgw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3wgaxrjte.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3nwqftcfk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3xzhmhryj.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3onizxjuz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3wznunikn.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3tgmygecn.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3usjxgnqj.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3ktpvdeyy.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3qlxakvwi.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3pxxsosbs.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3ftwrqyeu.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3zgentxze.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3fpacdgam.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3sfcqxygy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3lbigihlt.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3bstpgcsw.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3hjqgxnwi.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3dstudcae.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3qjfzyapq.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3zldaonhx.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bcrcenzk.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3fvzgmrfq.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3znpybvfo.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3ecpxwauq.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3twvhbhxc.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ughbqufg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3vekqvvib.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3ybptmgkz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ritmdqnr.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3sndiwgrc.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3hbithqsv.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3eyigrksu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wxkegfzj.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3amibfgsr.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3qejhhaif.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3dnjrgiua.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3lwvlriqo.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3mbbrdsdg.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3vzgmzyvy.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3xhpatwos.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3yejgdbbv.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3maqruvmo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3ywjbaaeo.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3yrwzxsaq.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3incstaxk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rfycpgmi.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3yyuwojjo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eayqvewn.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ojhnvkda.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3zcrwmwhl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3buytyeyv.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3rmpfyalx.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3sftwqyti.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3apktudjy.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3lntmieqd.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3hnbrfblc.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3dgwkvoek.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3uhfyvpbl.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qcytzuyg.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3tzwscwiu.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3cgcfbmcz.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3wzoruukp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3lchbsmzr.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3kfibemhn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3mtviwabm.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3cleygnei.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3fuilzqnw.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3uwcejruh.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3toubdaxb.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3yuucnnfp.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3yhocwpqc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3craoyfft.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3peyywzem.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3aplwkoia.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3iotaedqy.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3afutzagz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3uqybcqcn.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3davwmrna.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3kdcyojbh.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3zhaxhhxv.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3mztuehlq.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3wcsyhewj.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3csjowuuo.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3avvammba.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3daamrrev.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3vlmhvseh.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3creaxuqb.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3ybciejbm.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ikqanvep.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3ruqnbums.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3diwjajyj.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3ivmzssfo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3eukkwwks.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ccoadefq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3vojpihzm.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3tevovkbd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3jyzonfew.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3bmrpnwne.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3wwkpjnbw.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3qoctuggv.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3lzjqkmms.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3swbebkny.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3fwblrdcx.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3jmykswbm.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ysbpuknq.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3kweldxzc.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3dwhtpenj.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3sssczdfc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3olymmnbo.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3mkhieofj.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3pgtykgbw.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3mwzikgjy.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3rhynuqaa.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wizassis.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3larcignn.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wysixqhb.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xsfmvjab.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3nclmhxbe.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3iqhgubsh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kxzaqngg.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3xndlcpfi.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3tiahjfvm.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3hyixqvah.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ecylxosg.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3fpsxoigw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qsgriuzg.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3hyjceqoj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3pwyzuzmp.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3eajktkbd.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3klfmdcto.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3zckxufmo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3ssyksuwo.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3jejspvjd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3vjuzlupf.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3yrfvegxo.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3ocnwosyo.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3xiqbytid.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3akliciag.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3ghoxauif.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3tqlnbdag.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3wilhuyia.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3wrcxzfkm.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3vysrltfg.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3rhcbwxxt.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3nxmrxpdu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxaljrre.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tnyllnha.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3pfzpchqm.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3uhbyxwhm.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3afgvhavu.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3cuhwnnie.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3qmiuhzpp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3mxoywfvm.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3tmkugaaf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3pxqaefqq.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3gxuveixp.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3fspxpyhj.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3sftyrzgb.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3xsrfojml.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3sfgdxdik.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3osonalni.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3rambcopp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3qyowqnku.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3gzjtqiqz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3stvvlgnr.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3psdqypvt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3nzrducsr.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3jerckkfa.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3brztkqok.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3klhozgbl.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bbuqatlw.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3tgefekgj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3arlxrrrv.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3hllrdjty.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ciddzuwb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aqdjkwrh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3phsaextx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3txaoylkq.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3aaebkjtd.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mjoglqsm.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3gnvenoow.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3xuiuaubq.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3zmvzlhcf.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3smxmcouq.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3yqikrsvt.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3ojmrmaxu.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3ucxqkxfj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3gshmgdcz.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ijppxmis.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gzpmwwfu.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3maglcmqa.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3buzqskbm.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3khaocgib.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3uyblhfgv.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3pwulzqow.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3lsdtriew.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3kzashjbi.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3hosrhjcu.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3zghgsmfi.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3fdydkzax.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3ikpviomx.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zgqotwts.html


<!-- 参考信息 -->