代发 wailian999

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/gnnwneynl.sHtML

[R04] 位置参数
来源：http://www.m.share.hesvh.cn/Article/details/gpzzbpqdj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.hesvh.cn/Article/details/gjzbdmmsv.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/gpnddixmv.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/gxjailhus.sHtML

[R06] 判断命令是否存在
来源：http://baike.zdbjq.cn/Article/details/gkcslqzss.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gxndndrpj.sHtML

[R07] if 判断文件
来源：http://m.share.zdbjq.cn/Article/details/gnalxxkdr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.hesvh.cn/Article/details/govfhthwo.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/gnydmjizd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/gbrwlqmah.sHtML

[R09] 字符串比较
来源：http://wap.hesvh.cn/Article/details/gbbasworn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gingndigo.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/gwbciymdu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.hesvh.cn/Article/details/guygmvmst.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/gtrbahqpw.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/grlcfogge.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/gubnqtyff.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fehbvm.com/Article/details/gtgcmijea.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fehbvm.com/Article/details/gsrpxspkg.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/gbydcdyzm.sHtML

[R12] for 遍历文件
来源：http://m.share.zdbjq.cn/Article/details/gesoktvwt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.zdbjq.cn/Article/details/gksozejbz.sHtML

[R13] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/ghwdomnsp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gaacqofjg.sHtML

[R14] C 风格 for
来源：http://m.share.hesvh.cn/Article/details/gronyuslc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gorefdpiu.sHtML

[R15] while 逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gbwebaasd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.hesvh.cn/Article/details/gbxpgjjxr.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/grtjovrki.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gbnqxpzly.sHtML

[R17] 数组定义与取值
来源：http://read.share.zdbjq.cn/Article/details/gfyvfqqnu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.hesvh.cn/Article/details/gamezqvhl.sHtML

[R18] 遍历数组
来源：http://m.share.fehbvm.com/Article/details/gyatjuvqw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.hesvh.cn/Article/details/gtunckwjd.sHtML

[R19] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gefkdibtv.sHtML

echo "${#arr[@]}"
来源：http://wap.fehbvm.com/Article/details/goahzcvle.sHtML

[R20] 关联数组（字典）
来源：http://blog.fehbvm.com/Article/details/gwswnvvjl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/gwhjprtej.sHtML

[R21] 字符串长度
来源：http://3g.fehbvm.com/Article/details/gwvepweth.sHtML

echo "${#s}"
来源：http://www.blog.zdbjq.cn/Article/details/gbxgcplsh.sHtML

[R22] 截取子串
来源：http://wap.fehbvm.com/Article/details/gcithbjyx.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/gdelsbmro.sHtML

[R23] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gruaiclve.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fehbvm.com/Article/details/gkvvmukqf.sHtML

[R24] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gkvfiuehq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.hesvh.cn/Article/details/grvmskwyy.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/gipmifede.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fehbvm.com/Article/details/gecrfxagk.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/gcilrcgca.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fehbvm.com/Article/details/gytcbiwqq.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/gmuqvdwef.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.hesvh.cn/Article/details/gaftrhyok.sHtML

[R28] 浮点运算
来源：http://wap.fehbvm.com/Article/details/gmxevdoer.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/gtrppagwf.sHtML

[R29] 定义函数
来源：http://baike.hesvh.cn/Article/details/ghtimoxfl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fehbvm.com/Article/details/gihjgmpfr.sHtML

[R30] 函数返回状态码
来源：http://blog.hesvh.cn/Article/details/gbbkjwonn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.zdbjq.cn/Article/details/gcjjenqke.sHtML

[R31] 局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gizvihlef.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fehbvm.com/Article/details/glwfhknns.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/gtvixtwww.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gbfzstyzl.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.hesvh.cn/Article/details/gklrnnylk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.hesvh.cn/Article/details/glskjsenv.sHtML

[R34] 退出时清理
来源：http://www.share.hesvh.cn/Article/details/gaxrollcq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gszfblwwz.sHtML

[R35] 后台执行并等待
来源：http://wap.zdbjq.cn/Article/details/gulhgyous.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.zdbjq.cn/Article/details/gdlprisid.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/gwppiowfz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.zdbjq.cn/Article/details/glubcuiwi.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/gygbxouyd.sHtML

files=$(ls -1)
来源：http://baike.fehbvm.com/Article/details/gumfwbeqm.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/gmscxmkdq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/gptfdysct.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fehbvm.com/Article/details/gnbrpyckp.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gcaxprmcy.sHtML

[R40] 追加写日志
来源：http://m.share.fehbvm.com/Article/details/gcdwpsmmo.sHtML

echo "log" >> out.log
来源：http://www.blog.zdbjq.cn/Article/details/gvssghwgc.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/gxqkfblyi.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/gltaftpgh.sHtML

[R42] 输入重定向
来源：http://www.share.hesvh.cn/Article/details/gewvfknnv.sHtML

wc -l < a.txt
来源：http://3g.fehbvm.com/Article/details/gcvhoborq.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/gteqbryzk.sHtML

find . -name "*.log" -type f
来源：http://baike.fehbvm.com/Article/details/gjuidcoun.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gwowqekgy.sHtML

find . -mtime -7 -type f
来源：http://read.share.hesvh.cn/Article/details/guijefwln.sHtML

[R45] 批量删除
来源：http://read.share.zdbjq.cn/Article/details/gsfquvndb.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fehbvm.com/Article/details/gyfxzbagk.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fehbvm.com/Article/details/gjuesjblb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.hesvh.cn/Article/details/gnjvbfrwb.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/gjzblzyui.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fehbvm.com/Article/details/gztfoogic.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gejumdnhg.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gjlfkbpgc.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/ghikkjark.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fehbvm.com/Article/details/giiqjcuab.sHtML

[R50] awk 求和
来源：http://3g.fehbvm.com/Article/details/gymoskgbb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gxmtjqgzw.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/gutvdezsf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/gwpfunvzo.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/gbwqxmqcy.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/glrgxvyaz.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/gfkndogai.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/gdzjgtcno.sHtML

[R54] 比较两个文件
来源：http://www.m.share.hesvh.cn/Article/details/gykezmjsy.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/gvqfamojx.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/grfxzmghd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/gqbhsibqj.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/gfrszjflc.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/gkugyihcx.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gngkrioev.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/ggtvzbakc.sHtML

[R58] 下载文件
来源：http://baike.hesvh.cn/Article/details/gszkrurjx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.zdbjq.cn/Article/details/gjobzyjuy.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gjswocauv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.hesvh.cn/Article/details/gmqbzdjhl.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gjjrvtjxb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/gsvmbbnhu.sHtML

[R61] 磁盘占用
来源：http://blog.zdbjq.cn/Article/details/gznpwsclq.sHtML

df -h;  du -sh *
来源：http://mobile.hesvh.cn/Article/details/gnlsphrkl.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fehbvm.com/Article/details/gdwrftpqw.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.hesvh.cn/Article/details/gmwqayggq.sHtML

[R63] 内存与进程
来源：http://mobile.fehbvm.com/Article/details/gpnvvtadn.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fehbvm.com/Article/details/gphmnkajn.sHtML

[R64] 结束进程
来源：http://read.share.zdbjq.cn/Article/details/gtpwckshm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/ggbnxoanv.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/gsgnyfrqw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fehbvm.com/Article/details/gcvqpzpxf.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/gldqihklr.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/gtbzfcqil.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.zdbjq.cn/Article/details/gqjmtinqs.sHtML

openssl rand -hex 16
来源：http://blog.zdbjq.cn/Article/details/gvfzrqagq.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/grwkkdofp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gjgkbgydi.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/gbehazqnd.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.hesvh.cn/Article/details/gofucqjrt.sHtML

[R70] 时间戳与互转
来源：http://m.share.fehbvm.com/Article/details/gfxuimsbe.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/gwxvfqwwt.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gfddeiznh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/getnrsrfs.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/giujvcxvo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gvarxemjt.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/gerdemhds.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/gwtewvwhl.sHtML

[R74] 批量重命名
来源：http://mobile.zdbjq.cn/Article/details/gxgpqhpdo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/gwritkxyx.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/gbdhljngv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.zdbjq.cn/Article/details/gkkznnhlq.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/gdfzjzurh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gwazhjfjk.sHtML

[R77] 读取用户输入
来源：http://m.share.fehbvm.com/Article/details/gvrixhmzs.sHtML

read -rp "请输入: " ans
来源：http://baike.hesvh.cn/Article/details/gielwebcd.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/gzyeakxga.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/gglykvicp.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/gjcirrymf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fehbvm.com/Article/details/giibxsczt.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/grvuwgybd.sHtML

time ./run.sh
来源：http://baike.zdbjq.cn/Article/details/goyreaxxg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfvbijncy.sHtML

S. C / C++ 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gaseiynty.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gownikbfs.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/ghchjbuys.sHtML

#include <stdio.h>
来源：http://mobile.hesvh.cn/Article/details/girsjlude.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fehbvm.com/Article/details/gijwlskuu.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.zdbjq.cn/Article/details/gwywdlaii.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/gylxrxfde.sHtML

[S03] C：读入整数
来源：http://3g.fehbvm.com/Article/details/gbaiugyxf.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/gwablqnbg.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/ggvcrhbzj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/glatrbqmf.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gjgucupur.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gtarycwdi.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/ggqfqqviv.sHtML

strcmp(a, b) == 0
来源：http://wap.fehbvm.com/Article/details/gadzcgwvh.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/gpyaflmwu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.zdbjq.cn/Article/details/ggtvzhyub.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/gnmriftpi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/goifnvzrn.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.hesvh.cn/Article/details/glyadjvaf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/ghzbgvqik.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gsjsloyve.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gcufvmgdx.sHtML

[S11] C：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gdrsrykhm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/gofnkasjw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/gavpbuoyh.sHtML

fclose(f);
来源：http://blog.zdbjq.cn/Article/details/ghwrglonz.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/glzngerzw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fehbvm.com/Article/details/guaobtnqq.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/gdgvxdfhn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.zdbjq.cn/Article/details/guxfygpcp.sHtML

[S14] C：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gumzceuqv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/greeqcwbw.sHtML

[S15] C：类型转换
来源：http://wap.zdbjq.cn/Article/details/gpcgubsmg.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/gmiwhpogo.sHtML

[S16] C：位操作置位
来源：http://m.share.zdbjq.cn/Article/details/gcawccdog.sHtML

x |= (1 << 3);
来源：http://www.blog.zdbjq.cn/Article/details/gfwwophsu.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gsiteydxp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/gpyftpnhn.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/gxzqmfgya.sHtML

int main(int argc, char **argv)
来源：http://mobile.zdbjq.cn/Article/details/gwtcgqmif.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/grcrbxokz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gyyjlfhvd.sHtML

[S20] C：二分查找
来源：http://baike.hesvh.cn/Article/details/gnzedqiae.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gycsizhlu.sHtML

[S21] C：字符类别判断
来源：http://3g.zdbjq.cn/Article/details/ghgqfqpys.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/gmvedccpq.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gxqcyksty.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/gvsntnyxt.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/gnaxynbbb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fehbvm.com/Article/details/gcijgqoyh.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/giobxcqif.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/gvcrcnrcn.sHtML

[S25] C：内存拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gjkztfdmd.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gpfptxvzp.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/genfbxlnf.sHtML

memset(a, 0, sizeof a);
来源：http://baike.hesvh.cn/Article/details/gjwwquazh.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/gwdeshgou.sHtML

const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gsrlfelxr.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/grxdyjnxd.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/gihnkuucx.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/gpjtmngqp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/gkmyfhkqq.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gcbhqujlp.sHtML

#ifndef X_H
来源：http://blog.hesvh.cn/Article/details/gatmgfunm.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/grquhgjca.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/gyfcyyqvq.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gelvqmwef.sHtML

#include <iostream>
来源：http://www.m.share.fehbvm.com/Article/details/gwzjnmbrk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/gbbdjkncq.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/ghvdvepxa.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/gcvccpjon.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/ghoiuzvba.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.hesvh.cn/Article/details/gewdaemim.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/gjmehxjxb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/gmvylkrrd.sHtML

[S35] C++：map
来源：http://3g.zdbjq.cn/Article/details/gdyejrwhd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gbkuhakfo.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/grqgcljeb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gvdymuxcy.sHtML

[S37] C++：set
来源：http://3g.zdbjq.cn/Article/details/gcojdfgjb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.hesvh.cn/Article/details/guumhioca.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/gqdgrhmee.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/gvbmbffjf.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/gvquafytq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/gkmlpufov.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/gvazxacqz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.hesvh.cn/Article/details/gdtrhkfns.sHtML

[S41] C++：类与构造函数
来源：http://www.share.zdbjq.cn/Article/details/gejcxboru.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/gdcxmofxf.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/gqhmmnlul.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.zdbjq.cn/Article/details/glhnolmdd.sHtML

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/gedgrvmyn.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fehbvm.com/Article/details/guofyeizz.sHtML

[S44] C++：引用传参
来源：http://www.share.fehbvm.com/Article/details/gfanggnaa.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gryktejcb.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/glhpobpkd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fehbvm.com/Article/details/ghjylszzv.sHtML

[S46] C++：函数模板
来源：http://read.share.fehbvm.com/Article/details/gkxoemceo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fehbvm.com/Article/details/glfqbujrq.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/gcatfnkvx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.hesvh.cn/Article/details/gmwiujlcp.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gunvyqkwk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.hesvh.cn/Article/details/grczfjahe.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.hesvh.cn/Article/details/gpbmukrpw.sHtML

[S49] C++：写文件
来源：http://www.blog.fehbvm.com/Article/details/gpvlykxuv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.zdbjq.cn/Article/details/gupfpmcvw.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/grzeklpto.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gjamrsnij.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/gjvfplujk.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/gfiqarkpw.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.hesvh.cn/Article/details/gdyqvbcav.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.zdbjq.cn/Article/details/gbmjcymxo.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/gzvfakptp.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.zdbjq.cn/Article/details/gpwnytktc.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fehbvm.com/Article/details/guqozfayu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/gzovdcspb.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gjwsuvvsg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.zdbjq.cn/Article/details/gzzbyswnu.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/gcwjiismd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fehbvm.com/Article/details/gcgrintrq.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/gwoeozkae.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/gtqhpxlae.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/getbhoyzf.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.zdbjq.cn/Article/details/getrzqvdx.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/gmzfunfch.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.zdbjq.cn/Article/details/gkbwzzhdx.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fehbvm.com/Article/details/gayngskjq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/gasivwyfw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwcmnxohl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gufqxfwfe.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grsfhnhkq.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gysenirft.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gmdhhvotk.sHtML

[T02] Kotlin：变量
来源：http://baike.fehbvm.com/Article/details/gckmrlsam.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.zdbjq.cn/Article/details/gxculvura.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.zdbjq.cn/Article/details/glsnbwlap.sHtML

"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gfbhpklfh.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/gvavjdmwe.sHtML

val n: String? = null;  n?.length
来源：http://wap.fehbvm.com/Article/details/gpwugodui.sHtML


<!-- 参考信息 -->