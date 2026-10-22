代发 wailian999

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2ojlbpscw.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2lfbeligr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2xtfhieli.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2zsvtoiqw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2huumdtwt.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2wjkagcbb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2tndwwqlp.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2rppjeptb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2nfvrftvc.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2mkbmyqlu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2kvdsirrn.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2djdxcxcz.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2frynzyyn.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2einyrrcj.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2kahgpane.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2hknecege.html

esac
来源：http://www.52xcode.cn/Article/details/gt2lftvdzsj.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2sjpiryqk.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2gxjhkgjg.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2zysimfyl.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2eywybvyd.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2udlsyoqq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qvhfgxjf.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2kcwfntnr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2ltujafxj.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2yrbkazme.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2sobabpvu.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2ttydwdnc.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2nplgqjjv.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2xqvoiksd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2blypnyrr.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2rgpvldsy.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2obcuhyjo.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2eirecyvy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2rmqpvtev.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2paphpcsz.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2pifpwabe.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2pzvqfeyg.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2uvybskiz.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2eabgezlx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2xhxswiwj.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2bklwejjh.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2lvlnyhfr.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2wfjiikzo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2dmogoroy.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2axfklmpi.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2ysoygxmo.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2mnskytyg.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2nuoslogk.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2jpptsmdz.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2jkemxety.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2qxneodpr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2lhnjxzga.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2opqmlboc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2xccijxhb.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2cwodmkef.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2auxkxknu.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2ncevtges.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2trozvscr.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2cflligpp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2ifysyoqs.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2drvwoonx.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2mwsofbyf.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2teepteej.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2rgqpbwhj.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2scjdpcbe.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2ozsnuchd.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2ypeowizk.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2ygiuhkuw.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2zonfbads.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2gxgjmubs.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2mecbqjyu.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2nneuuang.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2wgyskrpo.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2vhvxdqee.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2asrnbjae.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2vrbdhiqt.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2hloqcgws.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2cmtnktwj.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2heuxonlb.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2htrwerld.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2oiynnwve.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2gbhniiiw.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2yqjfvvta.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2wmnbyvbr.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2zimzyiyc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2phosovey.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2rscidgci.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ymfhjnjk.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2jmjohpat.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2lzbepudm.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2qvtgurgv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2csezdtbj.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2scppffyk.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2lkasebpc.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2nhnffcoh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2cmgepiga.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2wwlagibd.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kcvxsxkp.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2vuvcnyhk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2qwxpdwzs.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2pyvkxgse.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2dvcovayx.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2qhjymqeg.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2qppnvnci.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2wxzhwgbb.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2wslfovrx.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2yigvjszs.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2lmfooinc.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2hdxqeczj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2omobcycy.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ujmvilnh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2dstjahvq.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2dcmgrzpr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2ifszxrrt.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2ibvatznh.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2mjpjnypg.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2gyhvuopc.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2ptnigyyh.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2klemhrjc.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2eyqliutp.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2xhiamzdz.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2wczzziag.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2odenxmna.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2jywmwiwa.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2dcggwxcl.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2ssewyzbl.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2ghwaurgf.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2dgbohpyk.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2yluiwdzp.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2vdiaoaox.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2bbpimypq.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2nzivxumy.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2gauenhkd.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2uaavhtkj.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qdenukcx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2wkfhhfyb.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2whwvxrbg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2mcthlgmm.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2kiyocpnb.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2slybocbr.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2dypnccal.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2zudtmkvf.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2vbqggmfh.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2mprbfcvx.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2qmjpefhy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2vhdforxo.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2kkjwssqp.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2bfjjkkxg.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2ktbbwlqv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2diyfcpnr.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2jfwfhwti.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2kgzgemol.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2rrucxsji.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2cuobhhcm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hhhsfbxn.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2wmqbxhkw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bkmdafpl.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2uzgsamoy.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2enosecie.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2jcucadjr.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2lxrhrwde.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2pkglhmtm.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2nfnbhqkl.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2pcrmqblq.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2qlgutwow.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2qcrbyedj.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2qxskhhqe.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2xonugjqr.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2szsyqbmk.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2fakcdhip.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2fwfqeeov.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2zlnduegb.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2jrcwgjrd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2yugrppfm.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2fijagvmv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2cxutftms.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2mojkxrjx.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2xkphshws.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2viqipvzc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2dqtrdhnp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2gvmhbhid.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2gbxddpaq.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2vjaujzfh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2djkizbpw.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2ubhhhgcu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2kunxwren.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ihogxfqn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2dkzflnjk.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2vszbsjpg.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2bozdojuw.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2wlbngkrm.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2utqwgtnq.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ketmdfri.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2zsebjugl.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2vefooqli.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2eatmmcxs.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2cmwkdody.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2absczjwb.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2vottxusg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2imzznree.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2kyehatji.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2rslngdrh.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2adeilzdf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2xkasrejq.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2qtyqurio.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2jiimplca.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2hmsvubts.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2zegcwbdl.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2lgrvwsem.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2zicpthfc.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2jssqxybp.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2vhloclmx.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2xogzadkb.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2uuwqhbdn.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2jafsooak.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2yexsbpzt.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2epskbexx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2dpirnhjr.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2oyjqbcdx.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2yajkceel.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2wmpmglxl.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2trkcqjta.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2twpfkrhr.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2ixqipqyj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uhcydsib.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ehrsxtwx.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ghbytodl.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2yxhlfytm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2afjzlbkk.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2cimwdojg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2agzrphyf.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2iklralkb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wkoxougr.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2ffftrnfh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ycymdege.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2rddfekwa.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2oraklblf.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2gictqdoj.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2wmfeowsr.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2rszbvrro.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2zjauvpdv.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2eipnhddw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hjsxenyt.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2avawujvy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2hmmzomee.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2xpjonhwl.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2ifxxuesq.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2eowmunih.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2mzssvebg.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2xhlgozcw.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2csguhdxp.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2jqeaagxv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2brjlcvtg.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2qlxoxqdk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2pzupuspw.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mwzwgqvq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2wzitpkbr.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tcjizros.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2swbfaehv.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2kolcgdlo.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2arajnkfs.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2yrkviwqk.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2voehfhun.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2byggtigf.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2nowjtsmo.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2ysijmucf.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2tcvdqtmm.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2sruarnqv.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2gcmnvtcs.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2rulykctp.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2atdryjpb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2cgnhfiwb.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2cfprvouv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2gbcodmhn.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2lwslvvty.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2gttsfett.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2kaxvvrtr.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2ismevjoj.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2vsjglbkx.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2usjzfksa.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2dzguacnp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2mkxotgyi.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2gehcsnee.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2tsjpmmim.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2igrtdrdg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2bojvumuw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fkecwlwl.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ibirydyz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2kscjaxsb.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2qgvkguor.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2pnpltrru.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2lnpebzqt.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ylruasdn.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2kagyxact.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2qgqmthus.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2bzqqmcuk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2owlcmorl.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2qcmjmffi.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2oumhepzp.html


<!-- 参考信息 -->