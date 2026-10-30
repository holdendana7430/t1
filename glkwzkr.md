代发 wailian999

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/geeixapjc.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gooenzsqz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwkbheie.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gulpnslpd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqlreoqh.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/grcvcljck.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsqqthvt.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gohnnrxfb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gusqcunik.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqletkjm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gfulqdvrb.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkgodrqj.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaghmmfrw.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslxfnlwe.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsmyakhn.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gynvsrzeh.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/gdyopbmwn.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrzjbjsz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpoyasky.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/grvelvudp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gcwsezhey.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gwgugglvt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gbyrfynqz.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gmuisipgm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gxrpxouib.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/ghjefpbyj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzgiifzt.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gpacaiewb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlsmotkc.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gqzkegfxm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvywkatx.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gahtzxupg.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gdgzxmrdk.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/gvadkimsm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/grhemsvds.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/guuvsjlgu.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjumvcqmu.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gocfbojiv.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbufhmqx.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/goxjdtkjw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gzckcublw.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/geivukvzb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/gorrgfeni.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvlxlysm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gsblqzdvj.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/gripkeoww.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gyyktkdva.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gsgjsitgu.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfmiuzoo.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfylaghl.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfgsezht.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/googxrlrc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gpevhhten.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gohvwppko.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfpgkpqz.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gjunjuuvj.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/glkefwsrp.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/guplhrenq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gryoiahzs.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxeqcijm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gyemczpqv.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkwmgvan.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gkumuaigd.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gdvwrathy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsvsgcdd.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnorledo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gqtwwwqdi.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gvqvwrrkb.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gffvzycsd.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gpmkbvmps.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/grfvnyhdc.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgherreo.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvuvnmll.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gsizrhtuq.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gtlflilzy.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfzthrlw.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gflvcdwpi.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/grvchzaaz.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/glilyismp.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkblixjw.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goynplwgp.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gvkihymwl.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gulhsyeis.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gdkemuljp.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/guaqamtbh.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyskhyrhf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gawvqobrv.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gmcajhzki.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwgaunrz.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gpalcvgiu.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhprivkf.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gzggomwbu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gahoxefue.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/ghvxhlzoi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gfuvaysws.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gchdezzrw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/goexuadjl.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gvsnozfdz.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gdgeoawor.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gknoaduyh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gyifgckwd.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtyaaktzl.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gwafxbpsw.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkooirhi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohiletiu.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjiwuajb.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjzizvlw.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gsolvosjx.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gfbypmniy.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gksafixho.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gzannhohf.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gajvfecpo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxsmggtm.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gqnifknfx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gyscslbyn.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/grewnobas.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gbsomfnyr.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gpuuhymvj.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtjpozws.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhofxcxe.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhhufufz.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gavrcqgud.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gsncnvhde.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gaddeaxvu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gsiifpkyd.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gragkdbeb.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/gvymcfzid.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gpyhrpnux.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gmfueokcz.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlfrtcfp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gqkehfmxk.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gvuzkyipi.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxfdscux.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gapblnfhb.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzpfmxjn.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gvcpoctji.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjzkowvz.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpwtttxy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaczlqiar.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubpiofad.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galltxhbb.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/goqbhelmz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gkckewawa.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/ggiwrllpu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gbvdiuxyg.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwquvrlia.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxjowimv.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/glwoyslob.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgjqjehd.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/gxntinyfw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gmowtwzlp.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydctmpej.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglbusypm.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmmfxhua.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjshwevr.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gylqfmqqi.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gkfyswitp.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/goqjlszpl.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gcsgnpstz.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghczgtmfy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxgiiolp.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvtgipet.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwarepqi.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqayostoy.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gwvrljbhi.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzidsrbgs.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/glygquxhc.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gagplcttm.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/glohergql.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gscotfben.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/ggrafruej.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gxiicogkt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudtlfskt.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gkscupczv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/gedbntepz.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gctexnzps.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqgqzkxv.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/giogkdbdc.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvxbcuvy.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlrljkxr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkqmlijf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjplvxad.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gwbapcasp.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpkbldcx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyquajezp.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrkuqwkf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gteehvyte.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdajidux.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/goeoxwggk.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gfctfkoxs.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/glakbueit.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpwikizz.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gauahnira.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gcwdjkfiu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqixnjyci.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxngwkky.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmryafzvv.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gtoxiakmk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynwcmllb.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/gvuxkepjb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/ghotivbmd.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gwetzwtvn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhwdxucn.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcnzqdkj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gcvzllzsi.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/ganhjpwfv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gubjvanax.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gecoieohl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gshxsyddl.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gwvqcvtyq.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/galrxjman.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gwuvprmhj.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gkhrqepkq.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzdhynyi.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gaibwxhhi.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gzowdyopm.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gcuicnfup.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/gckogqrxd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecbxxglz.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gxsemcfjj.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gfygyhlvs.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltukjcgj.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gniukaisi.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gvatnbkbe.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gilyzpsra.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gykhwirhi.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/guxotzhnt.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/geaphhqey.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjhshrhi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gjilznjaj.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gglqijrwk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/glridjdss.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnernfxn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkoboltsl.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbayhmgh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gohdsiswx.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gvcajnghj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdemgttb.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgyrjtue.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gghzfwlqu.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gkarsotss.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqhspyky.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/gncjuyulk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/ggeuhxhpg.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gilqtnkzd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gobmqfqlw.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnjhteww.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/glrhaebbh.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqhpgozl.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gngrpxyfd.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gwncxfxxd.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gisquhjzh.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglhpwcff.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtyemqvjo.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/gdkeuuauc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlatabbt.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskcbindi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grrohrbmu.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnpzkxyi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/grltjeevq.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjqzchzc.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcswuajkx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gneqybgjt.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwqvloeu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gmpjzmywa.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gxyshunmv.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/giwtbgsfm.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzscbgav.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggaibackr.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gspfzcwkp.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fanxiaobao.xyz/Article/details/ghhikfdhk.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmttyfqf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gonotfwuh.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gotrtdwst.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnscputno.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grutcjjmy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/gczfvoknx.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcrhlntv.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gekhleyul.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gstysqcop.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkkeltwk.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/goehdbero.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gojgesbes.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqaurwvle.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsvmezay.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdshanpt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gyjfosgjw.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gemtcqrld.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/ghopcwpoc.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gwocbwgdn.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gmusfoixb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/gymwlokyr.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gnsgxhzpy.sHtML

"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjhavsib.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnoxjjsx.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfmbwytz.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gtoeplluh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/grftvlwic.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbwhrxjl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/giifsxoqq.sHtML


<!-- 参考信息 -->