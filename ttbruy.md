代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3nppjchgs.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3fsaognym.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3yskylnea.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3kpbdctqe.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3tbbwhvrc.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3vvgzqbbb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3tzaaobgj.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3alurilfy.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3zslackfi.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3mjtgddli.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3kyhmdnvq.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3dkwkmjkg.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3kkbgzofo.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3fuqbujve.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3imuyukjk.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3enrtgzrf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3reswkpib.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3neladwya.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3oxxcgbyc.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3rlaibvof.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pjskcgsx.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3ihpkfrhw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3vhlnzikp.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3zrlummue.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3namsogzn.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3kjjlkahp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3nargfvva.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3fwtrwpfj.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3izyjddjw.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3ytlwtvnb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3aymvtecq.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3tqfqeoex.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3nudusyxh.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3hsgmhxxm.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3ynmeonuc.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ispnqyzv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3tjweddxy.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3bawnujyn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3xuiqehnv.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3dhvhzied.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3uyrfhjun.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3rvgdvqsj.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3vjilpvom.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3szzinpxe.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3kxjdwxiv.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3budtsolr.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3wrsjppmv.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3bpfkjhfn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3tjycgnvx.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ykjozrhr.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3saaauqzu.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3ucmyrihj.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rdbinnht.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3nkzjtnkt.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3tmjgklth.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3kdzhaihq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3yefjtfiq.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3xndjaggq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3lbrgzsol.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3vcnjgplp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3mvkoczun.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3oswslxmq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3dlfcuzxi.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3ybirtfcw.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3rjlilhld.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3mzpbtxzj.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3jlveisjh.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3ljopswwd.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3fvnyyfew.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3nahhezek.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3fwwimjez.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3ohjlkdbl.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3imtgzhok.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3oqngpijk.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3fogpixri.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3uzmnmoei.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3sjaolypb.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3yydcfpln.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3mcikoste.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3livpmnmk.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3mxvkdnlj.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3cfinydbp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3yacandmc.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3cackpscx.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3mrziqbab.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3yzthsaqz.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3glwkkaff.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3orwpclah.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3vtfdvduq.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3dhjwkput.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3brlzimgc.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3fbbifgoe.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3mvajafjb.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3yopgzaqy.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3iswrmyog.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3wciwliuc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3wpwynuyf.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3hnmqknkb.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3torxfwdx.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3sgybavsh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3fyhnahhz.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3zpbfweaw.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3nvddrtea.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3mqxvwvne.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3riiuobtt.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3jzbrnqhc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3ehlpzonc.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3fhqahptv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3ucoqckuk.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3qxpejpms.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3sqyrojvg.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3pvqbdqfu.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3zsoxnmem.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3dawaxvcc.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3wbplxfsw.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3dowwitqq.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3ackqtkuo.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3yiwtonvk.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3oczachfi.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3bwzkuldh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3zepcvveu.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3qcciuxlg.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3dcqzlneu.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3hyjmlksi.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3xllujwqd.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3jeyeaavv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3ctfpjgmn.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3khsgrqvj.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3bkxnujoc.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3qtsiwfwt.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3rfahcxae.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3bdzchrji.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3xnwpjjbt.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3rbmyapyy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3cwaaxqta.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3xzxveobz.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3bxpjxpvw.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3qtgukide.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3trfnxjmu.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3nablhrcd.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3mjmyulkb.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3llstyuxs.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3uzbteawa.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3ogqmruto.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3qppoycaq.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3reaaocbx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3qgjvbmzu.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3wrzrsjee.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3qoytpeze.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3yngyxewm.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3kgbtbijy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nxbvsrip.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3spmbnqym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cdksfxud.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fglncqvz.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3erunbdni.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3pthllity.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3oygznoba.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3bpohuaud.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3nzknfhde.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3uijgktkk.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3sftjfjfn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3svtnoxnk.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3xkoyfxtq.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zjgickni.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3alvggxul.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3dezzvpxt.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3czixtpey.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3zozaczla.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3tbezyzay.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3fpejxqal.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3qykbxxtn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3msuoezwg.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3ahgtptal.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3vjbxvltg.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3pyvufhcs.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3cgxsadci.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3bzqopich.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3eotutiqr.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3uzmfggxt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3fpjywati.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3zydbhhxd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3rmacclbp.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3oqfertwo.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3icjkoeva.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3hbdayhob.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3jnwycslu.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3gnolxsbq.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3zstgtnbn.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3nxevkkqy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3rmxbonvd.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3lwwctgnm.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3kusekdjx.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3hbwazbue.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3dkgimpet.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3ubqqqkom.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3istxfeqv.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3petnlqyr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3alqgufst.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3nsiorcbd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3jrgnknnd.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3ckemrssd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3unewwxey.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3xgrvjlaq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3ycigiavz.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3mkhgpuss.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3buaqafmd.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3xwvsqpiv.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3nhkvsgkj.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3ivadddqn.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ybcwasee.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3qbwxjblr.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3utnzjijp.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3sfiitiwo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3bhtuxobb.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3irnxkjgw.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ixdppaar.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3ivjxqejz.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3oxtqcnpy.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uuxlyqss.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3dgwxycbi.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3tuynseih.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3jffzeyjb.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3rhfjjapd.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3cvldffip.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3dzuugmjk.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3wtionltf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3vurbbxwj.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ryqbnzjv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3bdcrcywc.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3mvbrajnz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tsprnfkb.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3knjtugry.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vdwcxrbp.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3eknjvqkd.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3vhpgefop.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3fpvoubua.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3poatuxmu.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3pefoxrtx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xviinbcc.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3sdkzuujv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3ogrgmocg.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3tyupiqwo.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3rxhlqskc.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3maxohenj.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3fkoiwinz.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3mhcfodel.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3tcqwicqo.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3qnpmpuhz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3jkmvuwor.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3jzocxtxl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3rajywxir.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3rlpqrdln.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugktcqkh.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fmjeqsep.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3vqpxtakj.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3dgseoqhy.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3hjcjafvq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3kzjksooh.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3rssnsfus.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3slcnozyy.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3jobjkqoz.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3hwmridwi.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3ibimraui.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3fvlihzzq.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3zgxkjzzg.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3cuvpuuei.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3qfqsndln.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3wamqnbwf.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3jdsekcnu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3qcwzszal.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3cfnrycjq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3dzeixsnj.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3axxbomyy.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3cviqmamt.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3fmekyixj.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jptqbmvo.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3lezlgpkk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3dszjhehk.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3twkmdtdu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3muoxactb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qolevose.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3tzhvgeni.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qumjgaie.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cqhwyxdr.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3fvjpxlbe.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3rdhgvgfz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3gfafkfxk.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3zpetcvpt.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3zipiosmm.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3gvakwmbn.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3tuztyaua.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3qkpmluyo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3tmkyhxjv.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3bcivievb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3flubxkfa.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3bofxvvkm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3jpmlynqe.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3zmrjhgvt.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3timqmfnu.html


<!-- 参考信息 -->