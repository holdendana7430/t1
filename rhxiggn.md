代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.zdbjq.cn/Article/details/ggelhisas.sHtML

[Q90] 生成序号列
来源：http://3g.zdbjq.cn/Article/details/gpokgtsuh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.hesvh.cn/Article/details/gmsqkcmbu.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzfxclyft.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/gemxsekku.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gtpbdgtmv.sHtML

[R01] shebang 与严格模式
来源：http://www.share.hesvh.cn/Article/details/gevnhkzjg.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/gtimbznil.sHtML

set -euo pipefail
来源：http://blog.zdbjq.cn/Article/details/gxoovnieu.sHtML

[R02] 变量赋值与使用
来源：http://wap.hesvh.cn/Article/details/gbfsjkdnn.sHtML

name="Tom"; echo "$name"
来源：http://wap.hesvh.cn/Article/details/gruawvjdh.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/gdpjmzlds.sHtML

readonly PI=3.14
来源：http://wap.fehbvm.com/Article/details/gkipjuphz.sHtML

[R04] 位置参数
来源：http://wap.zdbjq.cn/Article/details/gpahljbdg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.hesvh.cn/Article/details/gallrvyiu.sHtML

[R05] 参数默认值
来源：http://3g.zdbjq.cn/Article/details/gweeibdoi.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/guzrexkzx.sHtML

[R06] 判断命令是否存在
来源：http://blog.hesvh.cn/Article/details/gjswcbyme.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gfnjtkkoj.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/gaxynngre.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.hesvh.cn/Article/details/gwrovimal.sHtML

[R08] 数值比较
来源：http://baike.fehbvm.com/Article/details/gcoovbbwq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.zdbjq.cn/Article/details/gldnwaxaq.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/govorqlfe.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/giybwojcl.sHtML

[R10] 正则匹配
来源：http://blog.fehbvm.com/Article/details/gppiamjub.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/gfiodbmub.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/gydzfijcf.sHtML

case "$1" in
来源：http://blog.hesvh.cn/Article/details/gauoyvkfx.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gzmbpafhm.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/gxpujsygw.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fehbvm.com/Article/details/gkyumphkf.sHtML

esac
来源：http://baike.fehbvm.com/Article/details/ggmhexraa.sHtML

[R12] for 遍历文件
来源：http://www.share.fehbvm.com/Article/details/gjrcovgpj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/ghozrcqjx.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gflgxntaj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gngtzquoe.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/gyflduaze.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gofqnrwxu.sHtML

[R15] while 逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/guxlwebze.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gazdvckmb.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/gpkezvaht.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gbufrbboq.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/gqzgrdavc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.zdbjq.cn/Article/details/gdjsftxpw.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/gisrbjnzi.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/gqbmzbmyb.sHtML

[R19] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gktqwyrwn.sHtML

echo "${#arr[@]}"
来源：http://www.blog.hesvh.cn/Article/details/gvdssxkgd.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/gcaxymfhk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gllzcmdom.sHtML

[R21] 字符串长度
来源：http://m.share.fehbvm.com/Article/details/gclwnnidd.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/gubktlvse.sHtML

[R22] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gcwxwfufl.sHtML

echo "${s:0:5}"
来源：http://mobile.zdbjq.cn/Article/details/gwhqkhgea.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/ggisqiszv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.hesvh.cn/Article/details/gtnamulif.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gjmjgazql.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/gymzozphn.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.zdbjq.cn/Article/details/gsjdbqchl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fehbvm.com/Article/details/gcrudragh.sHtML

[R26] 命令替换
来源：http://wap.hesvh.cn/Article/details/gxbwrxxlk.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.hesvh.cn/Article/details/grfatvogu.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/ggwuwdcfj.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gafsggulp.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/gctakluma.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fehbvm.com/Article/details/gzkbpttlw.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/grjpvrcha.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/gswmkcjpu.sHtML

[R30] 函数返回状态码
来源：http://www.blog.hesvh.cn/Article/details/gvtghjyod.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.hesvh.cn/Article/details/gmzrweade.sHtML

[R31] 局部变量
来源：http://www.blog.fehbvm.com/Article/details/gtqeizbsr.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.zdbjq.cn/Article/details/guimjulzk.sHtML

[R32] 参数个数校验
来源：http://3g.zdbjq.cn/Article/details/gabpzaoub.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gjdsxlhqv.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.hesvh.cn/Article/details/gwuzfwhvi.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.zdbjq.cn/Article/details/gskephjys.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/goqkjxgrc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/glaoihpsm.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/gyddjzesn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/goejqildo.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fehbvm.com/Article/details/gexwwmbtm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fehbvm.com/Article/details/gesrspwbh.sHtML

[R37] 把输出赋给变量
来源：http://3g.hesvh.cn/Article/details/gzsfhnxge.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/gfmebnphf.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/gwgzajrgy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.hesvh.cn/Article/details/gawcqmahc.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fehbvm.com/Article/details/ghcgsumla.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/gjftyxdba.sHtML

[R40] 追加写日志
来源：http://www.blog.zdbjq.cn/Article/details/gyqojcwjj.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/gaddwbjva.sHtML

[R41] 丢弃输出
来源：http://blog.fehbvm.com/Article/details/gdwymigvh.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/gqpwwqonh.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/gzdjoeflj.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/gcqlnzqvw.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/geqjwntln.sHtML

find . -name "*.log" -type f
来源：http://baike.zdbjq.cn/Article/details/gbcnzwrjr.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/gzfropewx.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/gxzvgddpf.sHtML

[R45] 批量删除
来源：http://www.share.hesvh.cn/Article/details/gmvkuoqbn.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/gqiwogame.sHtML

[R46] 递归替换文件内容
来源：http://wap.hesvh.cn/Article/details/gtjuudhjd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fehbvm.com/Article/details/gtkhylyok.sHtML

[R47] sed 单行替换
来源：http://3g.zdbjq.cn/Article/details/gdxmffvnd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gnnfymgtx.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gyncwddov.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.hesvh.cn/Article/details/gpeymwiqr.sHtML

[R49] awk 带条件
来源：http://www.share.zdbjq.cn/Article/details/gsiocrrpw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/gkcijozem.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/gdfcupuvn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/ghobiafkb.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/gqfnnegxs.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.zdbjq.cn/Article/details/gasgsdzez.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/gnwfudstw.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gyyksngep.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.zdbjq.cn/Article/details/gcghikeua.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/gjighppns.sHtML

[R54] 比较两个文件
来源：http://read.share.fehbvm.com/Article/details/gfrtmcuaz.sHtML

diff a.txt b.txt
来源：http://wap.fehbvm.com/Article/details/grgpgaqcs.sHtML

[R55] 压缩与解压
来源：http://mobile.hesvh.cn/Article/details/giqnogkgl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/gqdgrrzrk.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/ggilssfai.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/gsxqwmhuw.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/ghtyusyhs.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/ghreqqyte.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gsjuniqef.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/gkwydpsdx.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gpferiwpd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/gxdofdpbg.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/glqlhnjan.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.zdbjq.cn/Article/details/gcyerwozo.sHtML

[R61] 磁盘占用
来源：http://mobile.fehbvm.com/Article/details/gnubbnmww.sHtML

df -h;  du -sh *
来源：http://mobile.hesvh.cn/Article/details/gialhtcyh.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fehbvm.com/Article/details/gpgrhwwdz.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.hesvh.cn/Article/details/gfjyfneji.sHtML

[R63] 内存与进程
来源：http://mobile.hesvh.cn/Article/details/gkzymflqr.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/glgmrdaca.sHtML

[R64] 结束进程
来源：http://3g.zdbjq.cn/Article/details/genpjppaq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.zdbjq.cn/Article/details/grnhczkjp.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/gxxcgrnbz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/goneyeflp.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gqcaxwrwo.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fehbvm.com/Article/details/gomamgqor.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/gmydwiurz.sHtML

openssl rand -hex 16
来源：http://www.m.share.hesvh.cn/Article/details/gzuepsnjt.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/gutwjcilh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gdppqyxwq.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/goakuchec.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fehbvm.com/Article/details/gabsainfc.sHtML

[R70] 时间戳与互转
来源：http://wap.zdbjq.cn/Article/details/grtnmikcf.sHtML

date +%s;  date -d @1700000000
来源：http://blog.zdbjq.cn/Article/details/gpskpevcy.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gmgurblae.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.zdbjq.cn/Article/details/gfphfynte.sHtML

[R72] 等待端口就绪
来源：http://3g.fehbvm.com/Article/details/gsbalfopq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/ghsqnuniq.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gpscrsuxa.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/gofcgtnyp.sHtML

[R74] 批量重命名
来源：http://3g.hesvh.cn/Article/details/gaozfhzcg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fehbvm.com/Article/details/gviawyjfw.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gpabaqieu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.zdbjq.cn/Article/details/gqvrxxcqk.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/guxkqmubc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gmokxbxwf.sHtML

[R77] 读取用户输入
来源：http://www.m.share.zdbjq.cn/Article/details/gzggyhgez.sHtML

read -rp "请输入: " ans
来源：http://www.share.zdbjq.cn/Article/details/grzqplnrs.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/gnpufdbqf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fehbvm.com/Article/details/gmurgvcud.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/ghtcxftlj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.hesvh.cn/Article/details/ggfjozhmi.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gwbdpjfjt.sHtML

time ./run.sh
来源：http://blog.hesvh.cn/Article/details/gybyegoum.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gsctoiden.sHtML

S. C / C++ 专题
来源：http://mobile.fehbvm.com/Article/details/glfcqcjcv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnwnebnzf.sHtML

[S01] C：Hello World
来源：http://m.share.fehbvm.com/Article/details/gusokqmmu.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/gbewzsvxu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/gzgelzwef.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/goszsilgw.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gyrfwanla.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/gydydiiom.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/giafhpiik.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/geizrjzie.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gkhpcbuqh.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/gvnhajsaj.sHtML

strlen(s)
来源：http://m.share.fehbvm.com/Article/details/givdgazby.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gyzugiwjh.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fehbvm.com/Article/details/glmqewkli.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/gdjkltiew.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.hesvh.cn/Article/details/ghexosbae.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/gwnnasgha.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fehbvm.com/Article/details/gcyskpyem.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/gwfneozvw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.hesvh.cn/Article/details/ghpusoslr.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/grutlkvnc.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/gspygntjb.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gapekuxow.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/gylbkzskw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fehbvm.com/Article/details/gryhtlere.sHtML

fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gafwbxqfc.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/gpcyximta.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gwrhqbaxv.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/gqpknimje.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.zdbjq.cn/Article/details/gohuqilpl.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/gunaixjcg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.hesvh.cn/Article/details/grxxylnpz.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/gveuybkkj.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/gjbuojijo.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/gwhanetia.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gaopdlhhy.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gpcefbjeu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/gbjaeueud.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/gchrujecz.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gvovsjlky.sHtML

[S19] C：快速排序
来源：http://www.blog.fehbvm.com/Article/details/gsbsqygkh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gqcjaugyv.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/gvkyivojt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/ggnhzifel.sHtML

[S21] C：字符类别判断
来源：http://www.share.zdbjq.cn/Article/details/givpnkqzz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fehbvm.com/Article/details/gfemdiyxk.sHtML

[S22] C：字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gkhgeybrg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.zdbjq.cn/Article/details/gsfkqdhsd.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/gwnwpfjuf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gltwhrzhv.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/glkfhjjap.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.hesvh.cn/Article/details/gegqhdlox.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/gekudouoe.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/gnfklican.sHtML

[S26] C：内存清零
来源：http://wap.zdbjq.cn/Article/details/guboplphs.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/gedoyzrac.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/ggezweqxk.sHtML

const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gpcruyyuh.sHtML

[S28] C：静态变量
来源：http://blog.zdbjq.cn/Article/details/gxyywqawr.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/gfjuqsnwc.sHtML

[S29] C：变参函数
来源：http://m.share.fehbvm.com/Article/details/guljlsbru.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/gaodihxke.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/gkxsypvaf.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/gqhrfrlfv.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/gtvxflffr.sHtML

#endif
来源：http://www.share.hesvh.cn/Article/details/gakyfigsb.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/gkdjnftmw.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/gzwptsrvh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.hesvh.cn/Article/details/ggyeujlmj.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/gwyheqptu.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/gpegjbldc.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/gdqlgkrye.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/gujblnasr.sHtML

[S34] C++：遍历 vector
来源：http://baike.fehbvm.com/Article/details/gbjlznqnp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcwozqqvh.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/gsduvbzwg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/giayjouik.sHtML

[S36] C++：unordered_map
来源：http://read.share.zdbjq.cn/Article/details/gtanamjaz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/grhvkbsda.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/gtornlvvz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/ggtdhurwt.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/gswkfpusf.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gyrpiggiw.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/gunxxrzog.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.zdbjq.cn/Article/details/gftzeiitu.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/ghyfzmjsq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.hesvh.cn/Article/details/gwbwvuufg.sHtML

[S41] C++：类与构造函数
来源：http://3g.zdbjq.cn/Article/details/gpnglitfd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/gsnqqxsyr.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/gnvlwfird.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fehbvm.com/Article/details/gspiedixo.sHtML

[S43] C++：智能指针
来源：http://m.share.hesvh.cn/Article/details/gqaezeisk.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/ghrckntzk.sHtML

[S44] C++：引用传参
来源：http://blog.hesvh.cn/Article/details/gdrrkdfyv.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gzogvhipa.sHtML

[S45] C++：lambda
来源：http://baike.hesvh.cn/Article/details/gywpclmhe.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/gethoennb.sHtML

[S46] C++：函数模板
来源：http://mobile.zdbjq.cn/Article/details/gnbtswnvo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/gcdzippta.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/gjjsdfmwa.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fehbvm.com/Article/details/giormxhbq.sHtML

[S48] C++：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/grsepiebu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.hesvh.cn/Article/details/gtltkxrsc.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/grjfvgsgr.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gbdcbzbnn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/gthhjrdbo.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fehbvm.com/Article/details/gkejkjfik.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gdgkdlstd.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gloxxrppq.sHtML

static_cast<double>(a) / b
来源：http://m.share.hesvh.cn/Article/details/gfxvsrbtg.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/gngeehoaa.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/giuvzmvzs.sHtML

[S53] C++：移动语义
来源：http://wap.zdbjq.cn/Article/details/giunfosir.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/guirpiehe.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/gatsfadij.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.hesvh.cn/Article/details/gsjxycerw.sHtML

[S55] C++：结构化绑定
来源：http://read.share.zdbjq.cn/Article/details/gkkfllwgw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/gauvyvcya.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/glhbqxtps.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/gsawcvpor.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/gasobjuch.sHtML

constexpr int N = 10;
来源：http://m.share.fehbvm.com/Article/details/gkupqiesm.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gxnikkurn.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fehbvm.com/Article/details/ghfzpvlgp.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/gwqfqpcyq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gsoggzzui.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fehbvm.com/Article/details/gklbfxdpz.sHtML


<!-- 参考信息 -->