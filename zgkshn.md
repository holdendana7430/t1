代发 wailian999

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2zkydgblw.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2xlqepdxp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2mqgexctt.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2dsmfuwgn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2fmrwwmfh.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2brrqjrzo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2wmmrhofa.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2hdnehuvm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2ntsygkcy.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2cdlsljzw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2heqhxrhp.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2pzxfxmve.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2jugdoole.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2jouvrwbn.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2jafcciaa.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2idcfmcfm.html

esac
来源：http://www.52xcode.cn/Article/details/gt2vgqalkzt.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2twfhcqou.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2quhpfufn.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2mwnpnbde.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2yajbprcx.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ivgmuleu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2zawsgycg.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2zcjudzjd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qbyizzfk.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2ibnbnqef.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2twhoxuwh.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2qqjoopmf.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2nwgdaadd.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2badbhnsz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2wivuezvl.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2tiraxhdk.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2pnlpubgg.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2jqgwwtpp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2lqauhwxo.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2zfdwpdtp.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2vdithuhb.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2mfyjmnky.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2nxfagejh.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ugnqerri.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2mtfjhvtk.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2oznwyvvd.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2nkaombmo.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2vgabyxft.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2gurloebh.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2zfpluiph.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2bfzwjgzu.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2miekfpia.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2pxgdxzme.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2adgqkakm.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2irypuvfy.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2mrtkwxjh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2rtddizjl.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2sgpjnqpb.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2pqumehgy.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2bwnvnhmt.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jfzxuybt.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2tkixvwbk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2hqprvidx.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2prsmyfgd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2sfvwvgmf.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2foxogubj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2hacfbnst.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2ignqdfha.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2tmudslii.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2emafrnas.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2qvowzapx.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2hnpomttj.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ckewjvla.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2kneqyvnb.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2jtpujaoh.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2ohvuwvkl.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2gwcbccfw.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2qhclatvk.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2xcyywslk.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2dwakjieb.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2gctbzrte.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2avfhztpt.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2mgrxdkfg.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2ftmnsrue.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2jsjxkgtn.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2ynplpkby.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2fvazquum.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2xqrauwwp.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2ejzmdcey.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2jictmdeg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2kzwxeuuj.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2ohhhxnxx.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2josmucvs.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2nokemlkz.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2jygzugjq.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2rxguxfap.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2glesxmvf.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2czusvjns.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rufqkden.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2cvcgwggc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2bttomebg.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2dnkepshi.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ashuaxbr.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2hrhkbusi.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2hpmpewcw.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2aledicdi.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2sopogjyr.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2jhwjbwih.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2caudjvtu.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2vvasukxj.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2bpcmxawc.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2rkbzkumo.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2jceipjhl.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2tomkrrdf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2uroxqyzu.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2tiniibuj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2ikbeoyee.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2xutpwebq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2mpwbjkpt.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2rdvjvdii.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2ctqwldcq.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2jzhujhoe.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2dsxzusce.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2fmskkocq.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2ycbszqqa.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2ivroupaf.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2sjxnqaca.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2cwuxxnkx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2zwlyltqj.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2cbhfwfdk.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2mztanpai.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2khfuqfaq.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2komibqjj.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2reotqvgp.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rlojpqqv.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2yukaeksv.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2qxevbyrw.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2nzddwtio.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2szyztyvp.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2xtovlzga.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2beeojktt.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2ikgqgivt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2reatohym.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2fopsivls.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2bbmnvxan.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2bfgbtcvu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2sghscoea.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xdzmcych.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2mzywepdv.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2jhjcipda.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2onnfdwxf.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2avnkyebm.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2sbxhgukl.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2bselzpap.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2njaigcvo.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2nieynmus.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2kdmzmjyn.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2avpdgqkc.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2ruhmqali.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2easwbqkw.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2autcihjl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2twsmnpbu.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2skmbwumh.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2vxosyxao.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwvefkuq.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2zkgyytay.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2bwydjjuf.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2pxenazle.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2ahkavlwe.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2rcgaupnn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2grwwrzxk.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2jjzdunua.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2kzezdggc.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2wtugwrgx.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2yivfouhc.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2hndkxeal.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2univvjvf.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2tugdzjgv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2uefetvzs.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2dabotulj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2cibjaftc.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2osmgelqo.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2jxkdsawt.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wwrzmzav.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2thvxqyve.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2okmltxdg.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2mrxmyxvg.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2uvuxfxna.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ypcoqxvj.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2ztclyzsi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2fjcxfexy.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2rqifopva.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2kusvvjhp.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2fxdxuohj.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2xxdapblv.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2dwaabxhg.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pdttebpa.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2afifcqah.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2tsibbznq.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ikcaesoc.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2zpqopvjt.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2oqdwlxri.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2drcrjodg.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2ckqvytkz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2rotbnmrt.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2iatdrctl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2zvksmniy.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2limudwpo.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2aqhpahgj.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2dcspawal.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2nmpyfeus.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2rzsfxtkm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2ibdsiyqy.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2nxnztico.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2cbqsyteg.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2sfbxwtdk.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2gyjjsqoj.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2cxgbsmya.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ejtqocen.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2ujmvvcsb.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2owudwzkn.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2bqsgqtpz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2qqjjnwha.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2gonyxajp.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2eokocxkr.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2gvuqbbjb.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2cxpfbkzm.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2heusfdzd.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2qrdmvhbj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2ixygkdix.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sonexjjf.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2pqjafmwk.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2xryzerve.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2orbdmmaa.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2gcvandbs.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2bwmppwjz.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2pkizqqrm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2uypjdohf.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2kxbsbblm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2mcyevzwb.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2swvvosks.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wykekzim.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2izxomfkc.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2bjngbayh.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2ucanqcvx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2tzyditpz.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2gomcuuox.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pzaecxsf.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2zfseurkm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2uiihadvt.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2anvfmrvh.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2bivbmicl.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2rmdqbosy.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2wbzavlod.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2jxqkmrrv.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2kmugtzri.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2bvzqloew.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2wegrjrjv.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2egjsluih.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2nzaeedxj.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2njcezuaj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2xjsbsmdt.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2nuhlzvrc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2outgdouj.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2xcgzehtf.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2aazevocr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2mmfhkwdl.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2wpuwryhy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ihvnwyqz.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2imwqubcn.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2mtlzrrhz.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2tzlkakar.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmaxqodo.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2mctiyekg.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2wnodwwtd.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2urkeqnrs.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2qzkuzypw.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2pbywrltb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2efikmqlk.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2ubkfooim.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2nxtevpvx.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2fwybuuaf.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2hcvhofmo.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2dyiewlad.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2zwksybto.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2wrivhppk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2gztejfok.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2hrgnoloj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2tcipixdv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qksyfrls.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2vdvefyxy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pmijnzgn.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rgeqspuk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2hcgttfcd.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ausuehrj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2qdvybjfz.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2mgzgqbdw.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ttztwenj.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2aqltydrx.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2kkgjmwkl.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rhyawzjr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2coysbtxg.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2gszbyege.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2rfgygppa.html


<!-- 参考信息 -->