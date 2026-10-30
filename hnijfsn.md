代发 wailian999

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsftxbwob.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/galmujzyo.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gccusmcrs.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmoiocxcj.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gzniqtoss.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/gzdvywxae.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjshzpyn.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzhkwgrj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gifuawdpg.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gphwvgjqk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gorlvtetx.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpyeibol.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gvgnaqicf.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/grrbrqchi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/goqieslcw.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/gqltlcouz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/garnhkbgt.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcevlisou.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gtsqnruja.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gjamtppyq.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gefkdftuk.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczgwfjya.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gahokzwkn.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gvgjplnmj.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/gapqjurzz.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gosewpemj.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmbvrzrp.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/ggtusmokr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbktufmzg.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjsihqtw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtzbhecp.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbuqniyd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvluuuqbp.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxhldoac.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gvfrkehfn.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gkbwrplun.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvyrniix.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gjdilxbaj.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxdmxuvg.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhrqvrxr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbjadwvf.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gevgbdllo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihyltvgf.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gjuwblljb.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcforzkvd.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/geetpmxkb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpjhooky.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydfnlzma.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/ggsdsfvag.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gxreexgtz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gklxbqgdg.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjlvwahf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/glxlsszzf.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqyqfgnd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gktlotvgx.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gafuvkzyl.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gtdlarmcm.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gyicqjmnd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvzrpefh.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfshsruw.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gahiuokya.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gttyyiuhi.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfobbfhf.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbvyaukb.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/geiuyohse.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/grwohpqyb.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/ghojpdffz.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzoekhyo.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrvybsxv.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gqnnqnmxm.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/ghxieyplq.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gcdfuzbtc.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gbrvtzzia.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfillwlh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gryarqzkj.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/ggczajipo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gvmehfrvv.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/glasmhyox.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gltlhtndl.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpobdhoxj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gokfdqadr.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gixyznoto.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/grwldwzrz.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gznvnllws.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/gsjlgtlmb.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gbffkxczi.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gijvqawlj.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gnetifjnt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggeiyhgai.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gapusbeqv.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gadofjpnt.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gzgobnksn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/guaprqxqm.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gtyfrirxu.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrxwbcsr.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlhgwpzg.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvezbernl.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrtbhvuy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtusscqsf.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnaqmrguv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gunoapgtb.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpiduazlo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobjrbrzm.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gduffidwq.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddbeovzj.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gulcdlhre.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gdslxpnkt.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gstulkhop.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gxrgnygtl.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gkplxlgas.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gpwyghzem.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/grhvbwruc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlyqpsiu.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmahzlkm.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gunvzitgz.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/ghqsaotzf.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gitkbqpkj.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gdyooqmei.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gaepmbytt.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gouevpfnb.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gzujanfhi.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjcyttmm.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gbklkjikr.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gwxbeblla.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpnqdxcw.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/glltlemfl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfyrmdalr.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gqhyhttba.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlfynnzd.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffnobjfp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gkucdxyub.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gojyntvrl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gxtfklpum.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymirwinz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmrbkqed.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gpyhiqnhd.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/goobvhzqw.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjesodbw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gxknfzobe.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgwnbvit.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtmtblmj.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/grrjzskwi.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/gylfthsln.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyynebup.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gpavpilob.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/glfqbgwzy.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gabwtdcdb.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gksvyelse.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyrtvcck.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gsccwgcwb.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjvboays.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gqjjihfin.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsmewseq.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gougqcyvh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/giewruzfb.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkqwgmjr.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmiqqioqt.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gxybmtaip.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrjqzgio.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqqdgwsm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvgaqhcb.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/giycuxvpr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxngfxhnl.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/givvcaqvf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gatohdqvz.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduaftxdw.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gisqrihuc.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwpwbntu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gphygltum.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gjggktcpb.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmlaoebw.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqggmbyw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/glfafjqbk.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gqbxonzwe.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gvjtqdknc.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gradbfutj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gqeiohrdf.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsylfthvk.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjgklnwi.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gkhzepswf.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrakylwy.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvanbbdf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmigjdmsp.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gfywpebpz.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyogbuzku.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcwnyrtz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gvqaksfzz.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gglhdbifu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfyaiptjw.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqaezgwy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrajqxir.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/girrtjvcb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gtyuqsrcg.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gscajphjl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gyfynxmhf.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gtbvvnhln.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gbbcyjzmc.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmkhsopr.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpqjeqce.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gqochqwau.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/govdgpkpn.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/govmjdhgb.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gwtldmxjp.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gesimrzse.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcafnvpu.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/galxkhguw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/grzmckiri.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gilrxkrjd.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgtbtekk.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gednidxts.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gustsnoby.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjazgeyvm.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpkepdgl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gffslfvlo.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gvlnriled.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwxyfejb.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdohlrbzd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqnlgozv.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnvegxkj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwfmmdcl.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbwxdvwp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzmhujyn.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/grvhsimid.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gfhkcvbhe.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/grceatjul.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrddlhad.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsrgataq.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gxwhgpufp.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gnugfhcrv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gbdikctnx.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclpoypyj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/geaclncmj.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/gmwwuzfsm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/goxicvbid.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfehnaooc.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgjwswmk.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gmltsrqrb.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/gosftfgpm.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gwtmtvdrt.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gznhcwyfa.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmgqihab.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnyqgyahq.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/gdmjjjlfj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmgtiqowy.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcorpyezy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnzqspkj.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvqztglv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/gacgqtdel.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwiboihgt.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gkajespef.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gcpoxdnhk.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakuppfbi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkichgthk.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gmkeicerf.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gbngrwdeo.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/gtsmrzhaq.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/geswkutik.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/gwljgmrdf.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/gytwvzrps.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gacszhmmg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxahyxyc.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnundoug.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gjxswdzha.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrewqcui.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/gupkniicv.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftjpyrow.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gklbctpag.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/guosfryvn.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzxkjpab.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/gjxnhndop.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/gejxjwqdg.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/ghixlbqzm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqagsegm.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfsjfksw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyeselnj.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/glttijtfk.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkydemkk.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gvfvvstwb.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gshtxyxgq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/grdpewchq.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gstndkgta.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gcytozoip.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkzwfkxg.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/guqeszwod.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxjqhxih.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxxnonio.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gkyhpcboe.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwchavvhg.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdusklgh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/gwkxgpxan.sHtML

[T08] Kotlin：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/giwhfftnb.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gafusdkhz.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gkcwridyl.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gogqvjneq.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcukpaxlj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/gvevtcosc.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/ggtkoyafa.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqqhznkl.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/ggjephqct.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gzmwhurrw.sHtML


<!-- 参考信息 -->