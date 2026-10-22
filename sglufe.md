代发 wailian999

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2rqxqgbyo.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2udcopmdu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzgfpqtp.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2tthjujoh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2iewhxcxd.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2yxxsbzjx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2nwjldiis.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2fpafgsbt.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2fmnhaleb.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2ypbndzzr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ibkvfyuj.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2fwrozqwe.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2pphxadfu.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2bevpjbhe.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2htbftvcg.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2gnsxtcal.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2ixaakwmo.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2gbmubjhy.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2oxqqplwk.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2dcyyguav.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2wenvgxky.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2kzooynfp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ifgadldf.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ttpabdyt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2ubexucgl.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2vvkgsfgs.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2pbtrucxh.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2eybfrkjj.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2scjfcqjg.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2nkiadcpm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2uzulfvfe.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2xeyalnqr.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2yuqbcbsn.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2hfmqesaz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2ioxuouuj.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2dkeohnld.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2tjcflrpi.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2xgtpheok.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2pgiedrtg.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2eprwnxzc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2opokuvqf.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2caeuzyyh.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2bhrtviot.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2wgfsdfhu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2uczpzmqn.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2psuyleyo.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2ivtlbinu.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2jckgfkwp.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2llgikwmm.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2jiyizsrx.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2zgdqysog.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ganyints.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2rhvjyiso.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2xtuojxly.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2ctrrerat.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2gwgkcbqg.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2swatrwwk.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2lilwgvpv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2blkbnseu.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2lgbakemn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2mqwymhnl.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2drxzssgq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2lpteemaj.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2abelqzxy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2kvisiupt.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2callqzbu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2wnoridfx.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2mqukevak.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2owxjewif.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2tsfliqvq.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2dsgdroak.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2ctguoaxm.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2zsywmlxh.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2jcmkbimz.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2axfphsmf.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2ixrtssdu.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2hrxrvsfb.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2ckriofvt.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qrfgqmoz.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2tenzalnj.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2aooduyzm.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2iafuepnl.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2tuidnnlj.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2yikyvixi.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2lxggbiyk.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2vrzrpxir.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2caviplxn.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2dnomxlno.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wpxtjgkd.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2tnonuhlt.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2svwmzagt.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2tdhffgvq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2iwgsrsnk.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2zjjdqjlr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ncapigvq.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2pnykhdfz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2scrtxouh.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2kwvszdcy.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vmtbibky.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2itkpruzh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2gyvojdum.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2ubquguff.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2foneqnbb.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2dgrujexp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2ysxakipr.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2eshnihhj.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2llahvwqv.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2vohcyrww.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2uksbkiui.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2ihutfwop.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2uazwvwlm.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2qyrmfpah.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2lfleiqpg.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2zwjdvmqd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2runsqpwr.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2jqcxsmek.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2ijomfffx.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2qgspyriw.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2ksjtgpow.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2qyxzcbyl.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2fvdmtsyv.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2ptazkckb.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2fxvpxbaw.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2vqzcumdk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2bmnwdref.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2gjokcseu.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2gblucmvs.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2adpgklpu.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2abvylmqz.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2drmaucre.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nglmjtwz.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2ybfkvtgx.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2gterjruo.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2bjqowgcs.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2jsywtsbr.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2irvrveoy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2zpbemsse.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2pqpkvyqx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2nmmkprpz.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2kjneqrlm.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2hkrpvyqz.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2iobroajb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hojnnpoa.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2bajbwcmq.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2jxfwlede.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2wqwoqkev.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2qounzada.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2jyehxetw.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2ksththfp.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2cdliscqy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2phmyjjry.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2lfdpsjbq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2lhdptxar.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2vvsdosbm.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2tjjzbkaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yytdgafc.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2jsdgtgzz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ydnxolpt.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ofxbaclr.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2wriwwumc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2lnntcmho.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2xethjiib.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2avzyilqd.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2hwjdpodg.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2gooffaxy.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2sepkrayn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2tzpsrjfa.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2wpfylpcv.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sejkqpia.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2hyoudvpf.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2tywquujv.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2nysqmwcw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2hpbadioh.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2pibtmlut.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2ebpqsdzn.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ubinmbuc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2pvatobuv.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2eqhiafet.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2ncbkloxw.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2jdzsjksy.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2pyjnxuam.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2gdeenjji.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2dklwrdlg.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2lqcnvolb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2tvtjdsze.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2cuakcisn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2dbwleutv.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2dqenevhv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2tweytpep.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2ijmegulw.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2qqxetzjm.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2lfkfawin.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kivofnst.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2wuiuclif.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2qcyqnvep.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2wjbxxcao.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2enflxwmz.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2mvtrxlhl.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ykggxviz.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2leornwct.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2obghnemv.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2cgyxpamk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2dkecfamt.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2tfnrfuag.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2pxeaiktu.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2mbmskabo.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2bxgkiqcn.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2briogkev.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2fpmzwuei.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2lveixtlq.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2pwuenpdz.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2ymnisrxo.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2skyocojw.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2mbfpyafo.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jermhakq.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2ldmlsdop.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2nirlpdrx.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2ddqkvedk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2mueukmtm.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2wdycltcd.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2zrxqxzwr.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2fltzyptp.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2dojyxely.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2weygjyjk.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2swuxqhyo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2mfvycjpk.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2klavkjsu.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2cugmzyil.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2ltbzrruw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2owcalege.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2lpntbpbk.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2cfengbrc.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2dtjwgzus.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2luvkcudi.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2gafznxiu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2eqdznzlb.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2rxxlpqcb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rjotgrpa.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2eskmoior.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ixzjfens.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2qwbyynai.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2goxlaexf.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2tubjozxu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2hlixdund.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2czqopphh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2kvosjkwq.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2qbanpffp.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2ochovcrs.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2ucbztjoy.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2hntoweqi.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2surrdwpe.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2asrflsqu.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2hrglkria.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2mrtbwqgd.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2omsabqbk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2fppllylm.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2behdqwbb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2iokkiqvf.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ryaiyntc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2agnvupdh.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2shnbrirz.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2fllbcwfq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2igikztzb.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2cuaukoii.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2nablhxtb.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2jrdqwlhh.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2oqzeywej.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2rjeqhkzf.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2mdbywojo.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2vjrjqxhn.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2uiohnljo.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2poisuqfj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2chgdzsif.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2srtcqedb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qmcubife.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2qwgfhlea.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2qizdfvof.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2cqeabenq.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2aevncbav.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2glfczxbr.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2gagicxsh.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2hsaguofg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2stckpnja.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2noaoilow.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2xbrdxtve.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2krowdoyz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2cvyauthf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gylqzjct.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2npijvrkp.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2nwqdqmpp.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2eakzargx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2efvvrkus.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2eqludinr.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2yfszyiel.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2gneqkeqz.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2erniezhj.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2nnnqsvrt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2tvnwzdup.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2muagortr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2wtampmll.html


<!-- 参考信息 -->