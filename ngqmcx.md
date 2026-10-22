代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2qnqyputj.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2sbqelcts.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ielumnfr.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2wiipmkgs.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2heegasvf.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ehczurxg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2ijxabqcd.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2fwzzjrqb.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2payasrmw.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2bmvtazgq.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2rebrlhwy.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2ljhvnsbw.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2fhqyvsud.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2eovmogpg.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2zdnyjwbr.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2zgoajqoy.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2wvmpdhga.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2aoawjkmf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2vlryjyvc.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wkojnqkz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2awvnehds.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2lavzctvp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2gocogykw.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2hcxthrpk.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2qafmkghp.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2xexyiyyi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2demddfut.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2aceahvkh.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2xtwyxxaw.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2lyvyptju.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2wuteeaau.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2zwksrzgp.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2phtqgtdf.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2xdgifdug.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2feiquvsi.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2tavpudus.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2mwbitlhu.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2pvszsxxf.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2euhbpaks.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2ohkqijpm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2barjjzmo.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2laxokwth.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2cmpfhpnx.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2zckabzaj.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2lzpokjvm.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2rngzzhos.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2vforhycp.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2itpcyggb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2hypdkvzm.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2wfuyywee.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2jyuvhtkj.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2hezfrsli.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cerwgvqd.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2zbgoydwk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2edzdvgqt.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2aidetjlj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2clvtbtij.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2vdeestiy.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2mmdenunz.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ncaahyhh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2qrssxqrd.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2yfriucvk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2njgjnuir.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2mkeypsut.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2wbekqnkg.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2cegsongo.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2npppuoms.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2xzgxsnwl.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2cmxkziyy.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2zybhjtzn.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2mjqoqnar.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2msgboqbm.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2gjfywemp.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2xxntjumz.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2ygofftrs.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2yzjbgzhc.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2kikezdka.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2idctqrsq.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2tbclaypr.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2oeyswflo.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2tnywtwzc.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2nwrufxpz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2qihkigzr.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2crltgtlq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2kpqugxhk.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2nnuavhjq.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2oxksajcz.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2hlrmbghl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2iqrnlxci.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2vrfockpq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2gbhfwdmn.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2ltqgbbjt.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2dpfjwcxl.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2mspmdbid.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2zcoalgjy.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2qyyldcun.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2ysqvmhjh.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2sskcvahu.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2lposvoob.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2jsaayleg.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2jwjlgkbe.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2hztvmzji.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2ytzoekpt.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2ymkedxww.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2ydfcaewt.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2qfljsmkd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2nbjufpdf.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zcapmyrq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2atejihio.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ifsgkbul.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2njnwxcne.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2ggmhdrmc.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2garwbupu.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2rbdbpcap.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2feflelif.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2ubxhoxwu.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2hwcydlpo.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2ygsaspui.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2pxwvswjc.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2qkeffgas.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2ttbbfkvu.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2txfbzlmz.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2yyggiwhj.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2fobrxpza.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2oatrcvpr.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2rlbncfmf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2grcxwdvv.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2oycszvkf.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2fuwbnejl.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2mpocxnoz.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2bazyvicg.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2qwnyihcs.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2zpqlnsim.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2twdmknfa.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2beyuyogc.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2hugbfbco.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2zadlqjvx.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2ccadhjtg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wtkpggbk.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2zjcljibf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2ejvazgag.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2gysdqscb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2hyfrifnf.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2elrcexwu.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2dfkqymvs.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2ajtzqplu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2kcbfqugm.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2hledplrd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2egnvyvop.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2oeuxmbke.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2hepkltwu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2drlxiurr.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2imyyiufd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fnhubeey.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2habqbstd.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2tovgaqql.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2xkcnycyf.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2qzxqteym.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2zpquqipo.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2fpaqzkqo.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2xkezaozo.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2xjggcqrb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2rhitagiw.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ntxsgfyd.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2nktmequp.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2vcloiiin.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2duvejnmo.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2kourjylf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2tipedsrk.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2ygtxavxy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2kzinsnuh.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2jfhokxom.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2ptckvszn.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2asaniisf.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2pfnevxvr.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tmavhpnb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2nojngfkb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2atysfsor.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2lakvecpr.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2upvtepnp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2axtpdbpr.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2sbmiefbh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2llzngghm.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ltesdcab.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2vixsrvlo.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ccchhhzi.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2cksrzrcj.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2prsjcqmv.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kzfasyio.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2gpbyzbje.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2qzhsafda.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2yuehomko.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2dkallzqh.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2cmhxeomn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2iyjhxswn.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2ougiyoji.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2mxioesgd.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2quxgzivp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ultidpkv.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2wxbfeaij.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2vrliszvj.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2jirdopll.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2tkspbmkn.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2fzeydwnc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2uowoagfy.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ykwkfqkc.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2lorgtceh.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2jpoyueaj.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2vpjhfohj.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2fnwrxjfm.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kvjxfnvm.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2izmdkfsx.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2jlykfifs.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2oujnpkpx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2bgspnqvu.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2cyssqcmw.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2stwilhgk.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2wykkocwc.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2iroszhwk.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mulkxexe.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2cvnidvmu.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2ffzzvwol.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2dfafnndn.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2qlhtzqsv.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2lhllpjoe.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2rliekrpj.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2afnkeldz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2eaxuvztg.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2eyewsnvv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2syrkepzw.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2dxtleaeb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cpqwitww.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2zwoeupnn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2zlwyrhce.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2fxikkorn.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ddccnjjc.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2zkivgftz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2znehohet.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2tahkqher.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2crsyxziu.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ohhsglmc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2xcimbhfr.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2vjwkycrg.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2xkzddzuh.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2thmajkhe.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2efbpusfb.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2uvzueurx.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqaueulz.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2zdimngyw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2otjntwvf.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2gslujkwb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wutfexee.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2tnoraqkv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2fgjaldpw.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ucphehpj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2obcbnkhs.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2migfazgo.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2dlhccurn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2gulhnyhh.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2luoaafph.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xiafimmo.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2rxlrcyjl.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2kormabkh.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2ltiecrol.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2orkhqatk.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2qabhgedg.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2fqktnjrz.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2jvbjfbnf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2dwxaloen.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2atzhhpmz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2donnyvdy.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2dhvbgeea.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtjgoyck.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2bzafwbsm.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2wfzrtfmd.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2mdzcwdtp.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2uobxxkyz.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2jexxrmsa.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2iiuijmrw.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2yvntonad.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2dqqhzryv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hsozeddd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ugvkpkbc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2chvjfjam.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lpsmaacp.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2mxpuzlpl.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2ufezasmb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2nyjwlrur.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2cfylgsle.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2kltmztas.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2lefkymhz.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2katwyywa.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2uaoltuie.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2pozrrmba.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2kbuocyan.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2xrsjhkkd.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2yryrnvvr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2njtgiaoy.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2hsbfxpjg.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2qbzbubeh.html


<!-- 参考信息 -->