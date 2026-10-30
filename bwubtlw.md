代发 wailian999

R. Bash 专题
来源：http://www.blog.zdbjq.cn/Article/details/gbqkmbyiu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/golaudwca.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/gmgbpucza.sHtML

#!/usr/bin/env bash
来源：http://mobile.fehbvm.com/Article/details/gkneoqqbq.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/gzozjmjir.sHtML

[R02] 变量赋值与使用
来源：http://m.share.hesvh.cn/Article/details/gunwozofz.sHtML

name="Tom"; echo "$name"
来源：http://blog.hesvh.cn/Article/details/ghgqpiggi.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/gbyzqhlig.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/gbdbeplgw.sHtML

[R04] 位置参数
来源：http://www.blog.zdbjq.cn/Article/details/gaicohbva.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fehbvm.com/Article/details/gsfyoskvx.sHtML

[R05] 参数默认值
来源：http://read.share.hesvh.cn/Article/details/gmjgqxmdg.sHtML

name="${1:-default}"
来源：http://www.share.hesvh.cn/Article/details/gbbcovsky.sHtML

[R06] 判断命令是否存在
来源：http://www.share.hesvh.cn/Article/details/gkuevrksc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/ggqkwpixh.sHtML

[R07] if 判断文件
来源：http://mobile.hesvh.cn/Article/details/gmyfzpxpc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fehbvm.com/Article/details/ghcuminwv.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/grymrfppd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.zdbjq.cn/Article/details/glmsccreh.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/gnqrlndag.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gbyznpkil.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/gzxgeyfbw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/glcizdjgz.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/gyzdynqoc.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/gckslvevl.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gfrudzrap.sHtML

stop)  echo "停止" ;;
来源：http://mobile.hesvh.cn/Article/details/gnahwvsvp.sHtML

*)     echo "未知命令" ;;
来源：http://wap.hesvh.cn/Article/details/gkmnqsttr.sHtML

esac
来源：http://3g.hesvh.cn/Article/details/gylvgrfnb.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/gbwebetzk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.zdbjq.cn/Article/details/gkwctxhfx.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gosstfksj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/grrdvlzmh.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/gmakqzwjl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gojuaysxj.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gzilfnmul.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fehbvm.com/Article/details/ghlwvoecm.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/gujjkexmz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/ghchtfial.sHtML

[R17] 数组定义与取值
来源：http://m.share.fehbvm.com/Article/details/gbnbeqiqj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/gjqmlrwcz.sHtML

[R18] 遍历数组
来源：http://blog.zdbjq.cn/Article/details/guiwpjclv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/gwxuaixjl.sHtML

[R19] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gluyeekrb.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/gcyhzwmdd.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/gbnrqnjnx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gwsornxgj.sHtML

[R21] 字符串长度
来源：http://mobile.hesvh.cn/Article/details/gedjxzcir.sHtML

echo "${#s}"
来源：http://3g.hesvh.cn/Article/details/gdatcpzmt.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/gzfogwwhq.sHtML

echo "${s:0:5}"
来源：http://www.share.zdbjq.cn/Article/details/ghuhtxafu.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gxmxopbum.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.hesvh.cn/Article/details/grfzmapae.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/ganggeaau.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fehbvm.com/Article/details/gedwkemxr.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.zdbjq.cn/Article/details/gohvryvjl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fehbvm.com/Article/details/gvjaqxvrk.sHtML

[R26] 命令替换
来源：http://m.share.hesvh.cn/Article/details/ghesvwscr.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.hesvh.cn/Article/details/gdiumuebu.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/guhglrspd.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fehbvm.com/Article/details/gzejibmhh.sHtML

[R28] 浮点运算
来源：http://3g.hesvh.cn/Article/details/gbnfqvrgt.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.hesvh.cn/Article/details/gyohhsolm.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gkragyrgr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fehbvm.com/Article/details/gjrfzqbfc.sHtML

[R30] 函数返回状态码
来源：http://blog.zdbjq.cn/Article/details/gcqavhqma.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fehbvm.com/Article/details/ghsjbfyao.sHtML

[R31] 局部变量
来源：http://wap.fehbvm.com/Article/details/givqnmmue.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghulgyxyi.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/gdjpcrqwe.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/ggwkybsie.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.hesvh.cn/Article/details/gikpjeydd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.zdbjq.cn/Article/details/gkrhlarqy.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/gbgvrwkbp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/grgyqekes.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gkwaounwm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/gkvmdvbgr.sHtML

[R36] 并发执行多个任务
来源：http://baike.fehbvm.com/Article/details/gknjgyidf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.hesvh.cn/Article/details/gozpkkntb.sHtML

[R37] 把输出赋给变量
来源：http://baike.fehbvm.com/Article/details/gilctfbhu.sHtML

files=$(ls -1)
来源：http://wap.fehbvm.com/Article/details/gnztddxch.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/gzyyazadp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fehbvm.com/Article/details/gzorncyya.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fehbvm.com/Article/details/gmedmlbax.sHtML

cmd > out.log 2>&1
来源：http://blog.hesvh.cn/Article/details/gzlsxvrpv.sHtML

[R40] 追加写日志
来源：http://www.share.hesvh.cn/Article/details/gippeadmy.sHtML

echo "log" >> out.log
来源：http://baike.fehbvm.com/Article/details/gxojrdzgw.sHtML

[R41] 丢弃输出
来源：http://baike.hesvh.cn/Article/details/gncfazynf.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fehbvm.com/Article/details/gdlxrjybp.sHtML

[R42] 输入重定向
来源：http://wap.fehbvm.com/Article/details/gkxgszcbz.sHtML

wc -l < a.txt
来源：http://blog.zdbjq.cn/Article/details/gwjbzkgmh.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.zdbjq.cn/Article/details/gsqeeiygj.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/ggtwqcnul.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gmflmyygm.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/giinwrfru.sHtML

[R45] 批量删除
来源：http://blog.zdbjq.cn/Article/details/gxdbvmvxw.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/gbobcuhae.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/ghtwechin.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.zdbjq.cn/Article/details/glfstyaet.sHtML

[R47] sed 单行替换
来源：http://read.share.zdbjq.cn/Article/details/gjujxzryz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gwazmbmvh.sHtML

[R48] awk 取指定列
来源：http://www.blog.zdbjq.cn/Article/details/gpzmeffyw.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gemmepitg.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/giaxqqrqg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/gqyfzhfpl.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/gowkffweq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gbtcqnnvj.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/gzdvtclts.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.hesvh.cn/Article/details/guleboyqc.sHtML

[R52] 统计行数
来源：http://m.share.zdbjq.cn/Article/details/gceebpcoi.sHtML

wc -l a.txt
来源：http://blog.zdbjq.cn/Article/details/gtwhhbevm.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/gsepxxykz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/gsnjtymos.sHtML

[R54] 比较两个文件
来源：http://read.share.hesvh.cn/Article/details/gciakifsw.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/gjkqqcnqg.sHtML

[R55] 压缩与解压
来源：http://wap.zdbjq.cn/Article/details/glcadamtb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.hesvh.cn/Article/details/gvjkpigri.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/gysngvrfr.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/gptvhkfjs.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/gkyhrnuml.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/grceegpxh.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/gnkcbjsxz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fehbvm.com/Article/details/gkjowyvgf.sHtML

[R59] 发 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gmihjjcnt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.zdbjq.cn/Article/details/gpszmjsmf.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/gczvboxve.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/grqphscdj.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/gonspsgiz.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/gfilvhcge.sHtML

[R62] 找最占空间的文件
来源：http://3g.hesvh.cn/Article/details/ghxgzpxhm.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gywezksrv.sHtML

[R63] 内存与进程
来源：http://m.share.zdbjq.cn/Article/details/gaaawtpib.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/gttvyvuhp.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/gvyocqmiy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.hesvh.cn/Article/details/goclvgvsx.sHtML

[R65] 查看端口占用
来源：http://wap.hesvh.cn/Article/details/gkvlggmsd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.hesvh.cn/Article/details/gyuruxgfz.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/ggqjcmfrn.sHtML

crontab -e;  crontab -l
来源：http://wap.zdbjq.cn/Article/details/gnwjnguwa.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/guwjykfyi.sHtML

openssl rand -hex 16
来源：http://mobile.fehbvm.com/Article/details/gksmogutj.sHtML

[R68] 计算文件校验值
来源：http://www.share.fehbvm.com/Article/details/guznyzssa.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gwcilqjpz.sHtML

[R69] 生成随机密码
来源：http://blog.hesvh.cn/Article/details/gjkqvtxrx.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/gjvreqolq.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/ghdolstlz.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/gxztclsgu.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gkvnwowat.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/gbvbtbkli.sHtML

[R72] 等待端口就绪
来源：http://www.share.fehbvm.com/Article/details/ggjdpicdh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gnqoqsbqk.sHtML

[R73] 分割大日志
来源：http://read.share.zdbjq.cn/Article/details/geztlhnhl.sHtML

split -l 1000 big.log part_
来源：http://mobile.hesvh.cn/Article/details/gxwdotnmo.sHtML

[R74] 批量重命名
来源：http://www.share.hesvh.cn/Article/details/gzkxjhsgj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.hesvh.cn/Article/details/gnlsjzrhr.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/ggrvbulbk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/gjdbyzmpi.sHtML

[R76] 使用临时文件
来源：http://www.share.fehbvm.com/Article/details/gnjsymkkd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/ggeknmjrg.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/gwoezwtfc.sHtML

read -rp "请输入: " ans
来源：http://m.share.fehbvm.com/Article/details/gkdsxrgts.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/gnuplkyvu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.zdbjq.cn/Article/details/gnxplnkvv.sHtML

[R79] 解析命令行选项
来源：http://3g.fehbvm.com/Article/details/gvcskdwwn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/gyfnlzrfw.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.hesvh.cn/Article/details/gdqzmvxfq.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/ghayaflis.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gftljirdb.sHtML

S. C / C++ 专题
来源：http://mobile.fehbvm.com/Article/details/gpzuejbyr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdeivzqfa.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/gniygdakg.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/gebwpieva.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/gpmvsbsua.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/gxybublaj.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.zdbjq.cn/Article/details/gucxgulyi.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/griyezgzw.sHtML

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/gagndaase.sHtML

[S04] C：字符串复制
来源：http://read.share.zdbjq.cn/Article/details/gwyiviizp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fehbvm.com/Article/details/gkjppinwp.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/gvqrdnyrk.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/gxqzwkmtf.sHtML

[S06] C：字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gkeeoxvfu.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/giiwtkbsp.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/gummxdgjq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/gchxsptbh.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.hesvh.cn/Article/details/gxchfwgwi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/gdnpkzuvk.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/gopgzjvdm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.hesvh.cn/Article/details/gifoofjzr.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/giafbmuky.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/gwkmyguml.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gvemcfzfk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fehbvm.com/Article/details/gjpvxfxbp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.hesvh.cn/Article/details/gzhvczuio.sHtML

fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gbwdprvng.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gwskzmajz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gxbbfmrmk.sHtML

[S13] C：宏定义
来源：http://3g.fehbvm.com/Article/details/gcneovemn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/gazqwcmnd.sHtML

[S14] C：枚举
来源：http://www.blog.hesvh.cn/Article/details/gyzrstnqu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/grrastndr.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/gesrogxrt.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/gklznztpu.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/gvunwybsu.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gxxouzqxt.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fehbvm.com/Article/details/glrccrckl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/gcouoxeyd.sHtML

[S18] C：命令行参数
来源：http://mobile.hesvh.cn/Article/details/gdiywnfuc.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/gpbqigvjt.sHtML

[S19] C：快速排序
来源：http://m.share.hesvh.cn/Article/details/gydaxvnwo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/grrkqffya.sHtML

[S20] C：二分查找
来源：http://wap.hesvh.cn/Article/details/gigmwooyq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gebseqoyh.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fehbvm.com/Article/details/ghdwlhuju.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/gupihpuom.sHtML

[S22] C：字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/gghqbrvmf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fehbvm.com/Article/details/gofzdwxzm.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/gnxlohkbu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.hesvh.cn/Article/details/gxhofhsjw.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/gvfrlpqax.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fehbvm.com/Article/details/gtxlpxakl.sHtML

[S25] C：内存拷贝
来源：http://mobile.hesvh.cn/Article/details/gezzkgfhk.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/gtcclohbr.sHtML

[S26] C：内存清零
来源：http://wap.fehbvm.com/Article/details/gnxyatucb.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/gzwanmwcx.sHtML

[S27] C：定义常量
来源：http://3g.fehbvm.com/Article/details/goljrvwcd.sHtML

const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gnlwrcehr.sHtML

[S28] C：静态变量
来源：http://wap.hesvh.cn/Article/details/gvgdvoeos.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/gtyouihec.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/gkclulgyl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/gcnzwjpdl.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/gpqafvlaz.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/giairncvb.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gaizuqbzv.sHtML

#endif
来源：http://m.share.fehbvm.com/Article/details/gqkpvbtra.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gduugizbn.sHtML

#include <iostream>
来源：http://3g.fehbvm.com/Article/details/gyapkqeug.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fehbvm.com/Article/details/gxpldinrm.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/gflpvaouf.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/gwxxymxae.sHtML

[S33] C++：vector 增删
来源：http://www.blog.hesvh.cn/Article/details/gyycudzxr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fehbvm.com/Article/details/gyzfpumhe.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/gvklnsrpk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.zdbjq.cn/Article/details/gtqtpjobl.sHtML

[S35] C++：map
来源：http://mobile.zdbjq.cn/Article/details/gtmsayzdz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gquzrgdng.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/gxenmmecq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gumkzzyrp.sHtML

[S37] C++：set
来源：http://blog.hesvh.cn/Article/details/gwrldkmth.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/gtnglrpvi.sHtML

[S38] C++：排序
来源：http://3g.zdbjq.cn/Article/details/gtdrotitp.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/grvpgbwil.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/grwrqdole.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/glicqhykk.sHtML

[S40] C++：查找元素
来源：http://mobile.fehbvm.com/Article/details/gcikyomkg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.zdbjq.cn/Article/details/gsbtuvmmo.sHtML

[S41] C++：类与构造函数
来源：http://m.share.zdbjq.cn/Article/details/gwjxcsnje.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/gfxljpwvd.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/gvotobqvh.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/gcxofwxnh.sHtML

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/ggacksbtw.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/gclqcowbp.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fehbvm.com/Article/details/glwgjktfe.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fehbvm.com/Article/details/gfsivqvrk.sHtML

[S45] C++：lambda
来源：http://baike.zdbjq.cn/Article/details/ghfzbbudv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/gpztbjzpq.sHtML

[S46] C++：函数模板
来源：http://read.share.fehbvm.com/Article/details/gmzrlwdvi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/glzbtoehw.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/gjojfjngk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/gsroihhsf.sHtML

[S48] C++：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gmbeugplm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fehbvm.com/Article/details/gzvycmxdb.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/gbpcjnwls.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/gswhkpzmm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.zdbjq.cn/Article/details/gddspyfrp.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fehbvm.com/Article/details/gmhiyjcnc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gremifxif.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/gzvpihfgp.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fehbvm.com/Article/details/gjmfeyhxl.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fehbvm.com/Article/details/gseeydimy.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.zdbjq.cn/Article/details/gssgnzkxg.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/gmadrthwi.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/gxnthquzt.sHtML

[S54] C++：异常处理
来源：http://3g.fehbvm.com/Article/details/gpllxkgoa.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.hesvh.cn/Article/details/ghrsgmbyj.sHtML

[S55] C++：结构化绑定
来源：http://read.share.zdbjq.cn/Article/details/gsqdxpbkz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/gwactfklq.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/gcqfaiyfi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.zdbjq.cn/Article/details/gokxadwnm.sHtML

[S57] C++：编译期常量
来源：http://read.share.hesvh.cn/Article/details/gfnthbakm.sHtML

constexpr int N = 10;
来源：http://baike.fehbvm.com/Article/details/ggepxktva.sHtML

[S58] C++：命名空间
来源：http://www.share.fehbvm.com/Article/details/gckofmmzd.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/gqltuyxfs.sHtML

[S59] C++：静态断言
来源：http://mobile.fehbvm.com/Article/details/gctgezika.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fehbvm.com/Article/details/gwoyfozii.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gchwaocgb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/geoohwvyl.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmjqwryyo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/gbeanrftf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwktygnya.sHtML


<!-- 参考信息 -->