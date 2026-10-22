代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ihsrmgqf.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2hrmwuvvj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2vzpjhuoh.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2pvydjkfk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2hiufpduw.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ktpiwdhf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2swbkratw.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2vnjjshkj.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2nbszilul.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2vpednqip.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2soryhiuy.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2jfghwgmq.html

esac
来源：http://www.52xcode.cn/Article/details/gt2npztizst.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2hfisxflk.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jzxpotxj.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2pmnochml.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2olgokquj.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2xikrtjiy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2uelujcyw.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2drbwipnh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2ceatahrp.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2skhqeszf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2nueosryy.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2usgwvkgr.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2hxnepcmy.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2rojvwzei.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2abhdjnlz.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2dgnnwair.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2rwkzibdf.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2jwtvsqld.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2olrusmid.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2zlxdiyvs.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2jmchikzg.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2aibocnwn.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2hufapmpq.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2qljwywpi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2rgjxebno.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2hsoazaet.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2vekzfogx.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2wgeiihqb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2ovdajior.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2nftzhvhr.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2ylluzhlb.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2hnopjjff.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ecruegqk.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2hwzpcjal.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2rxjpdfjx.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2krdrnvuv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2hacaewra.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2wpkpjamt.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2dnuwzkhx.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2znriuflb.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2tnilmvpw.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ydhucvxb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2zdtcsitg.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2qyyezajo.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2lgniewhw.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2kglymvnw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2iqhgmmkj.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2fvjpitmm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2uyjzevlf.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2amcutyhk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2rykcvonr.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2wrzftckb.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2tlcrfklz.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2gqfilmmo.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2ifgjigew.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2kcmbzwpn.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2smzyhgto.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2upptkwzy.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2dvtinkfi.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2lsoyxpvz.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2juiqduxr.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2mqarkffv.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2wtntpmsk.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2acgufkui.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2xynwgeof.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2xdjhdxaa.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ezwnjuif.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2koxivvqh.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2srryobpd.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2cnvvwxcm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2ibsydxtc.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2zrrnvwan.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2chcehybn.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2zbbsaqhu.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ypdaawto.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2ixcnzaro.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2ofuknwts.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2ouujhwmg.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2tieznzxa.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2uqnoiqsw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2tvutsptn.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2xyoopzzj.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2mfidvane.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2ebachftj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2gqrmrztp.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2saaodvwa.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2evnqqrct.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2rumynvrs.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2kgaqvjcm.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2cyftblqk.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2tfwlattb.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2atwgqzxr.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2rojskbxq.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2hitxsspc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2csfgqefy.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2wnxtvqvh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2btdtqlms.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2nnecmvxt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2efskpatv.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2fztezund.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2ilrqdmit.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2jkgsnsvv.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2frxpfiim.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2hggnouip.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2zkljgbrv.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2pninimrr.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2oojkvnme.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2dqfrnyvp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2kcysopfg.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2tblbxljy.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2btjccnke.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2jesvkugh.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2duyxqafa.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2peczpyys.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2idogvmqd.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2grefzava.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2fckaqabb.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2pvcsrfik.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2fdzekmvx.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2qsbbubbb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2qpbigotj.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2pbgfhyve.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2vgjlujvg.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2waxxmtxx.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2eaynoxyx.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2uzcbhkap.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jemwsymv.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2sjrqolyr.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2hxyygecb.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2kncuafre.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2noqkjosp.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2cthwozre.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2vmsxjawo.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2gibcrucd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2tylawwqy.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2oexlrmor.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2uvrmbpbi.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2dkuyueoj.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2ksxgbspe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hpjncokx.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2tqbpdvhd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cqksaoud.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2iongkubl.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2rxkmuvbg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2fqeivrpd.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2skobqzck.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2brnrkvlm.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2soyorseb.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2kwboarut.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2ekjlifly.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2famczadt.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ullfbvwd.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2lkpzcqut.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ionkoejf.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2hxfzfezx.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2huvywday.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2tcsftuig.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2bzgjxzin.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2belspytu.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2zklvbdlr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2bxlpqsaz.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2jugjoopw.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2sgtfgmyr.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ynmrmvtr.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2rsbmhkuu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2vninlueu.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2rcbacunp.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2oitusdnn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2glhcudur.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2xenioszr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2agecqjxf.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2zjhcabpo.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2iclxrhut.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2vayssogd.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2apddcqlv.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2hxazwmmc.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ebmexkvs.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cdeuuaur.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2sgyqpxyg.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2uhotclvy.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2cgkkkehd.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2maofoalz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2qiddzumn.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2nbkgwens.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2knratklr.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2efbxucdx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2gnoevctp.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ypakhdev.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2wunpsfvs.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2qjlbkkia.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2bzqrgnwl.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2pjmoywvl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2hxafkelb.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2jdwbgpdk.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2snsnnneo.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2jfewkybf.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2vdbzwizq.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2gnbbrpbu.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2oqveqrav.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2fndukrhf.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2zrmjvlrx.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2qmlvjfmm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2ncfqsdal.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2pmwmsmoy.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2bjdjhmch.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2iakxqulb.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2gldrthuq.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gfzzdtze.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2muydnbjo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2lkgbsxzc.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2bbhadmsf.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2ggelkcjj.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2tpbrtuon.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ihrbyfkq.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2nfbajzig.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2jvrzmmrn.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2mssxyzug.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pjlgjefd.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2sbsqagcl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2cgirxbyb.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2vkyqxaln.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zkauyncd.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2skdusssp.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2htezwvck.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2rfvzndul.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2awqrnbdm.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2rzvfxqfw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2aewsloau.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2lygnefmk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2qaarzzlv.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2tifqgeda.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2fsvtstin.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2igpamjun.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2jtikjgps.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2ukugooua.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2oxzsloxw.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2wgfvqwzf.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2kywlagbg.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2zjgqusdb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fkcjrokb.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2bzgjvjkm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2umwsqqfw.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2bxnmzxzj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2rzxujmhq.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2sowigsfv.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2rvwmisop.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2nfiknrhu.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2tooukkzt.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bgjvgrug.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2twtsnxfy.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2bymvobfe.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2awmfepfg.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2kggmrofw.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2dofwzgxr.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2okzlbqtz.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2uasfcxxu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2fbojzqhe.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2qjnnswlf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2hvqyrcpd.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2jkeaarry.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2atiswulx.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2owotjtkh.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2nalygeak.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2qbmmnkbd.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tukzqphg.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2owlkipvz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2kiawuuer.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2jxxlcvzu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2oybsugcr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oecsukpq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2blgjceda.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2njbcjkcu.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wiqwqazz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wcalvlyn.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2cfnqyxoq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2zpkvtyms.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2gdkrcuxp.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2btrwdoza.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2zmzdfwtd.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2mcxzixmc.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2livpbhtt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2urlydmde.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2fhsxikdc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gtoedimn.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ddtbkeup.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2drwfhnrn.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2pgoyjoke.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2mltectfr.html


<!-- 参考信息 -->