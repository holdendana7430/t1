代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpicrgww.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/ghkvqbjuj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqmpjhxa.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gwhbkxrmh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvzgroxb.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzdadnir.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geruhfwgh.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyemllqre.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gsreowera.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gmjzwvgov.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkkdigjk.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdbsnxcp.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijgtbcxm.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gajrxhuyl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/garkyoabs.sHtML

[R13] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gfaufjclh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gvugqotkx.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttydjmfw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gtyqbqyop.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/ggpzelbku.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/ggalqpzdu.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggclbshjn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gunvxobbk.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gjtwjmmzx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/guawhtoim.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/glmxzqdxo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gatlmddbg.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/giibljsun.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gminsgdff.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/gljxndawl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gppvtmafs.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/guiqphgrz.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/gguysbppm.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gkykscwui.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/giynmnbnn.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gdvksszpa.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/gaxhgqhth.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvxwbllh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydzghufs.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxpcrngy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmbmgpay.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/gzctkwjko.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/ggjqtzark.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gueytoqgo.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gpooteowb.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gedewkaae.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gebvvomtc.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gyniyonbp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/gczntdhgr.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzckpjdki.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzpqcbwc.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwvbijxj.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyulcxlc.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzolutijw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsuffllx.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gsouheanb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gqelsebga.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprpkujbv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxgfvhgb.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gxccnzkwo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjuvehum.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwlfjltm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gzouptynd.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrxvprih.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gbnrihlth.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/giiirnwru.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gwphmtlgx.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdecnoru.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gpkkvrvvd.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbkbudiz.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/ggylvamgp.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gagtsuuor.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gktmytgkk.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gzsydldru.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gourylkfj.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdczawpsr.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gwmcfbajf.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/ghutjkfij.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbibyuvi.sHtML

[R45] 批量删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gekpvtczc.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghemwgopu.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gngguzqey.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gzhzogkwy.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gxelbvaoi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqairfsu.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/glrvbqywr.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gxobiovxc.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gwejkspib.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqumbvua.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gphzuszsj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxckqxox.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gdwejdgqj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvheikrs.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gjbtwoksh.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gvpqdzbwk.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/grjeyljjn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurxrmzgl.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdsakapg.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/ghbhaliwc.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/glgetnaxb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gbkrckadf.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gybywswrz.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gkfdeexgq.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gzazzwfnd.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxfmyvit.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/ggodqfsqh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/goigoyxvp.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gwyevbdyf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gbdvvehqm.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gbncsuwcz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwseyulf.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpzmaqzi.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdjpnyih.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/giwqsdtwj.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gsysxjqsu.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzoebqevt.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbumjosm.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gyjbptlvk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gpxmkljfh.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/gvfjfqaxc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcaefhza.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghftlhmkz.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gjyrlrjnj.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gvhnhpsko.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdomewtae.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gwjgcycyw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gpmkzzqwb.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwehjcoqu.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gomozveyn.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxwaqyxo.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gukysituk.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnykpjds.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/guwihgddp.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gpfjllthp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmnsdzvf.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gztannqpb.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvsrcdtt.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gzqgmmguv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhoierxz.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsxddpxd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpcaxbsc.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjjloade.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gsqdxucwl.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/govinhzou.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqoloblb.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gghssovgd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzayrxrtd.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejnsvqfw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gyeuxxsel.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfknqhbtd.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswrioiaw.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gppcreryt.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gboveshud.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guloldrjj.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gcctbxknp.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gazvwhbuo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmtrteoe.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gulvbibjs.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gtzdflkgy.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbdnwadq.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvshszvdl.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/gxrcuxrtk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gedcnfjbj.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsrfpwfj.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjamqybn.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gfrqikgnh.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvxinoiw.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/ghqjyusts.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gjyzplpun.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gcyhsnluw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecugjnyj.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqemjmyi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/giadmseeb.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/ggjcdgang.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/ggxnxkybn.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnejfxsa.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfcpfqpl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrvzksit.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffopuhit.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gkkngnhog.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gjguodtbt.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gagsntagf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gudsqhogg.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gueopptpe.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gskyxytpm.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gdrwuzvxf.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxozahtx.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/grsulqfhg.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/grgyqqudt.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgsrtrnx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghznmtzyi.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfmymwvn.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkstedxh.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/ginpwsyyl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbpgpuid.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjdfizzx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbciptvrc.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhvtowem.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/gjsxjcgqs.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/giizsqfdt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfonmhymi.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gjpakzttr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvetkslp.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gobatdybb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gtltkcidk.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gbicpogcz.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gostbsnkh.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpieeyoi.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gmopcrwjm.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpvmrtva.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhrvejgf.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnkkcrgd.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gmkxeyqjb.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcsmqenn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtwypzlt.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gjvljuvjv.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbazayvj.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqymaobno.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/ggvvduowp.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/grohzpbnb.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/guawxqlgk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gnrewbhfa.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gyhtxlroj.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqojtjihj.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gabifezps.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzapxteb.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdtlakvo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghhccazpu.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gjifgfxkt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjdpgfzv.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girrveeif.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjeocryzp.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/guhudgctn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/grefxicff.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/gvbmuhjut.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcmxqejq.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gnmygbzan.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybahzium.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gdneqdhcz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngjbufuc.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gluktgrzf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgqstgul.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gnpulscys.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gbizjsuqh.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/gydduvibk.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/goilwpmpk.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gcwcwhlun.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvmnpsjz.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmcbgydf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/geagzhfds.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjbtbjiv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnynkpim.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypybrxwd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gowzsjszc.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gletbofwi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/gemtztglw.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/guukcfruc.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gunffllae.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gcopbgpvk.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggujhuqob.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyoppqsck.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpmnvavr.sHtML

static_cast<double>(a) / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gugtwxflo.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/gvkqscqto.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgpkokab.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrjjdlhb.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmbbtqfl.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/ggomfrrmf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtptgqobc.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gekvjsope.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gjuncjzgp.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gqgrirang.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhygwlre.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgojhmjm.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjllxgcvo.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gscrtvmwh.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxkajiwt.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrwcznxm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdttgyyt.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gfouegxot.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjnnvvsm.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzcjfegv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/gpygliogm.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gytdqrcub.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/giawoobwp.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gwghmzslz.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gajyqeiqp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginreeifs.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/ggxhiewol.sHtML

"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guicaigvc.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/glicszdlv.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gaggareno.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjrmonvq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gqlaefhij.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkmifugv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmkfbhmf.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhobsymp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxcvamsr.sHtML

[T08] Kotlin：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gorsuptai.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gsmzpymng.sHtML


<!-- 参考信息 -->