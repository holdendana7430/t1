代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://www.share.zdbjq.cn/Article/details/gkiavobcb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.hesvh.cn/Article/details/gmoeqifbs.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/gmjblkuqh.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gakgfwisg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gozfjrjgn.sHtML

[Q90] 生成序号列
来源：http://baike.hesvh.cn/Article/details/gdyxlbmzf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.zdbjq.cn/Article/details/ghhnzwfpk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/giablwnlo.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/gmeuhqtxg.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggrebwgps.sHtML

[R01] shebang 与严格模式
来源：http://m.share.hesvh.cn/Article/details/gtkhqkjcg.sHtML

#!/usr/bin/env bash
来源：http://www.blog.zdbjq.cn/Article/details/gxcfkjilq.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/gkvzynofe.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/gvqmzkbum.sHtML

name="Tom"; echo "$name"
来源：http://blog.zdbjq.cn/Article/details/gccsvxirf.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/gcbhrsbdq.sHtML

readonly PI=3.14
来源：http://wap.zdbjq.cn/Article/details/gpqggxtlj.sHtML

[R04] 位置参数
来源：http://baike.hesvh.cn/Article/details/gzhprknls.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/gfanbgnmz.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/ghqbdgqxz.sHtML

name="${1:-default}"
来源：http://www.blog.fehbvm.com/Article/details/gwozblqgr.sHtML

[R06] 判断命令是否存在
来源：http://baike.zdbjq.cn/Article/details/guzksrrbq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gigfvhfal.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/gzindyskc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/gucgrhfae.sHtML

[R08] 数值比较
来源：http://www.blog.fehbvm.com/Article/details/gbffugibj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/gcuwtpnsf.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gtlnkisro.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fehbvm.com/Article/details/gdmrmnyaa.sHtML

[R10] 正则匹配
来源：http://3g.fehbvm.com/Article/details/gbqjmoncu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/gywiqadmn.sHtML

[R11] case 多分支
来源：http://wap.hesvh.cn/Article/details/glvgzmmmx.sHtML

case "$1" in
来源：http://read.share.zdbjq.cn/Article/details/ghjthjpif.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gwbnlwdxf.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/gwkzacysy.sHtML

*)     echo "未知命令" ;;
来源：http://wap.hesvh.cn/Article/details/gdnveomwy.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/gxccmoedp.sHtML

[R12] for 遍历文件
来源：http://www.blog.zdbjq.cn/Article/details/gchpjfolj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.zdbjq.cn/Article/details/ghpziidla.sHtML

[R13] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/gqcvhbugv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/guvpfhchw.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/gecywbllk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gnjawhmoz.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gyjqfhetj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fehbvm.com/Article/details/gkhykzdhf.sHtML

[R16] until 等待条件
来源：http://read.share.fehbvm.com/Article/details/gfjnksypp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gpcfwmjuw.sHtML

[R17] 数组定义与取值
来源：http://m.share.hesvh.cn/Article/details/grsqygpqh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gmttzcbfm.sHtML

[R18] 遍历数组
来源：http://m.share.hesvh.cn/Article/details/gwsbxccfe.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/gnwrynlxx.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/guehcrrxc.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.hesvh.cn/Article/details/gvjkbgxod.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fehbvm.com/Article/details/gbpvfyyiq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.zdbjq.cn/Article/details/glzupcvaw.sHtML

[R21] 字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gqmmqswij.sHtML

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/ghkkwssbc.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/gmsntfudq.sHtML

echo "${s:0:5}"
来源：http://www.blog.zdbjq.cn/Article/details/gengtiywm.sHtML

[R23] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gaczqrngx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fehbvm.com/Article/details/ggjllptwh.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gzbwnnsbd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fehbvm.com/Article/details/grrhxyqem.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.zdbjq.cn/Article/details/gwmnzpjpx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.hesvh.cn/Article/details/gcymdasvb.sHtML

[R26] 命令替换
来源：http://wap.hesvh.cn/Article/details/gzmprntbh.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.hesvh.cn/Article/details/gvsetpzen.sHtML

[R27] 算术展开
来源：http://read.share.hesvh.cn/Article/details/gumrgzhnk.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.hesvh.cn/Article/details/gwlzwzovj.sHtML

[R28] 浮点运算
来源：http://m.share.hesvh.cn/Article/details/gqvjhvkcw.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/gufqbkmpi.sHtML

[R29] 定义函数
来源：http://baike.hesvh.cn/Article/details/giykcdrsi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.hesvh.cn/Article/details/grphixuib.sHtML

[R30] 函数返回状态码
来源：http://baike.hesvh.cn/Article/details/gznenbopc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.zdbjq.cn/Article/details/gprthcsrg.sHtML

[R31] 局部变量
来源：http://www.blog.hesvh.cn/Article/details/gsdallspq.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/gmziporln.sHtML

[R32] 参数个数校验
来源：http://3g.zdbjq.cn/Article/details/gocvmjtyv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/glmxyznbz.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/gdgsubfor.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fehbvm.com/Article/details/grczxobgv.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gjacduplg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gxsmlffdn.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fehbvm.com/Article/details/gwxvygawv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.hesvh.cn/Article/details/gmgiejmic.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fehbvm.com/Article/details/gnwayltzr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/gspykfguu.sHtML

[R37] 把输出赋给变量
来源：http://m.share.hesvh.cn/Article/details/gzejozjxa.sHtML

files=$(ls -1)
来源：http://www.blog.zdbjq.cn/Article/details/geyyygtru.sHtML

[R38] 管道串联
来源：http://read.share.fehbvm.com/Article/details/gxcrgnqax.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.zdbjq.cn/Article/details/goagkklwe.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/gjxyvdbkd.sHtML

cmd > out.log 2>&1
来源：http://baike.fehbvm.com/Article/details/giizsgjly.sHtML

[R40] 追加写日志
来源：http://www.share.hesvh.cn/Article/details/gmsfdohjp.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/gslxrvwpn.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/gaedvxmkq.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fehbvm.com/Article/details/gyypksewi.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/gpehdsccq.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/gzdctvhqu.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/gtxmlrqfw.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/gvpstffgx.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/gpwhabpro.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/gqnernmpb.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/gkixomxwh.sHtML

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/gymvnrknn.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/gxnrjfxqf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fehbvm.com/Article/details/gcgvtfgxc.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/gmmitykjx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/goommtmsf.sHtML

[R48] awk 取指定列
来源：http://wap.fehbvm.com/Article/details/glmptykmd.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/grefxoybo.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/gmkrspaei.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.hesvh.cn/Article/details/gstfpssch.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/grbjdspch.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gcndegpue.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/gvgonmvsl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/gymwjvaky.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/gmkstcwgu.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/gktqxocmg.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.hesvh.cn/Article/details/gbuuzewmz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.hesvh.cn/Article/details/gfuenzzhg.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/gdskyxqik.sHtML

diff a.txt b.txt
来源：http://3g.fehbvm.com/Article/details/gxedqwyob.sHtML

[R55] 压缩与解压
来源：http://mobile.hesvh.cn/Article/details/gbsyrippy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/gbrfvgzcz.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/ghwybgvqu.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/gvchlsptv.sHtML

[R57] 远程执行命令
来源：http://baike.fehbvm.com/Article/details/gethogqzk.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/gtgbdevqb.sHtML

[R58] 下载文件
来源：http://baike.hesvh.cn/Article/details/gpoipeuxr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/gqgbxjsgb.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gnfwcoqsb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/glfhdxwhx.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gsdgzbhpm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/gjvntydoc.sHtML

[R61] 磁盘占用
来源：http://www.share.fehbvm.com/Article/details/gjibmoqyo.sHtML

df -h;  du -sh *
来源：http://read.share.fehbvm.com/Article/details/gigeudymu.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/gsmewhlyv.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.hesvh.cn/Article/details/ghskyjdag.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/gawjwbruv.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fehbvm.com/Article/details/gxrrhfzgw.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/gkkgnzmol.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/gcgkoifeg.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gihpdrklu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.hesvh.cn/Article/details/glmvkbfka.sHtML

[R66] 定时任务
来源：http://blog.fehbvm.com/Article/details/gekaxkdpg.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gcnbdpdfu.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.hesvh.cn/Article/details/gqsvhwrfn.sHtML

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/gedarifgz.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.hesvh.cn/Article/details/gchoxkpcb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/ghykdqbuu.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/gmooahlzm.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/gnfncsjkn.sHtML

[R70] 时间戳与互转
来源：http://mobile.fehbvm.com/Article/details/gksglqtsb.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.hesvh.cn/Article/details/ggplnfrmo.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gnfiritqj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/gbsglkuag.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/gskedytgx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gerdkiell.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/gftvzrpdv.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gbqnyxhjn.sHtML

[R74] 批量重命名
来源：http://mobile.fehbvm.com/Article/details/gffnanwmz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.zdbjq.cn/Article/details/gpucaqmzi.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/grpznipss.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.zdbjq.cn/Article/details/gabqztlsm.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/gpdtcvgah.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gqkitvbcl.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/gqejtrdfv.sHtML

read -rp "请输入: " ans
来源：http://3g.fehbvm.com/Article/details/goaudtbvm.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/gdcdvhoot.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/gjktvrsge.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/gbaclmmjn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fehbvm.com/Article/details/gccdwaffc.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/gwsmmedvf.sHtML

time ./run.sh
来源：http://baike.zdbjq.cn/Article/details/gtnqykmhz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvkgsvfzb.sHtML

S. C / C++ 专题
来源：http://m.share.fehbvm.com/Article/details/gorvxrocx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpsdkbxec.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/godthbpzb.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/gaexvysnj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.hesvh.cn/Article/details/gwhbxsemj.sHtML

[S02] C：变量与格式化输出
来源：http://wap.zdbjq.cn/Article/details/gysvcdgod.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gnsfjaooh.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/gfmwijghp.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/gufggezgc.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gvkhloutv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fehbvm.com/Article/details/gxjheorhv.sHtML

[S05] C：字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gaivgyryx.sHtML

strlen(s)
来源：http://m.share.hesvh.cn/Article/details/gkfmzosbh.sHtML

[S06] C：字符串比较
来源：http://blog.hesvh.cn/Article/details/gthrqjjfj.sHtML

strcmp(a, b) == 0
来源：http://m.share.hesvh.cn/Article/details/gdabdlbpn.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fehbvm.com/Article/details/ggvczykrb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.zdbjq.cn/Article/details/gqdaedbsw.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.zdbjq.cn/Article/details/gtxkmulsy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/gdvtsorsi.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.hesvh.cn/Article/details/girkykylp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.zdbjq.cn/Article/details/geggsyfkm.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/gztubhshm.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/gvzijqgqx.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gqfhvipec.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.zdbjq.cn/Article/details/gvjndcpml.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/gvdzitpji.sHtML

fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gmfpyklte.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/ggttrebxc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.zdbjq.cn/Article/details/ghuwmiime.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/gluicjcip.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/gcxxffdmh.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/ggkemrvpu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/giqqfpvvj.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/gccmaigyh.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/gjlxnnzvq.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/grnqkvwsu.sHtML

x |= (1 << 3);
来源：http://blog.fehbvm.com/Article/details/gtekevaua.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/ggnafaucx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fehbvm.com/Article/details/gfppfeucx.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gomvkoeml.sHtML

int main(int argc, char **argv)
来源：http://read.share.fehbvm.com/Article/details/gvdvjfgho.sHtML

[S19] C：快速排序
来源：http://www.share.fehbvm.com/Article/details/gygheukkv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gxdeezrjh.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/gomyzadof.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/glcbgrfif.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/gdwcoafmn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/gkrriecwy.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gvaubfrmc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/ggolhzkyk.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/gpudnacrc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/gmuwqzoff.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/gapscjoqg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.zdbjq.cn/Article/details/grtcyjtlz.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gnsiybnxg.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/gozwkkmrv.sHtML

[S26] C：内存清零
来源：http://read.share.fehbvm.com/Article/details/gphdyegax.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.hesvh.cn/Article/details/gxqkoerms.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/gxzurnucx.sHtML

const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gupxwsacd.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/glnozrfuw.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/gyigtnwej.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/gicyhbsoq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.hesvh.cn/Article/details/gqqohghsm.sHtML

[S30] C：头文件保护
来源：http://3g.hesvh.cn/Article/details/gyppbspph.sHtML

#ifndef X_H
来源：http://baike.hesvh.cn/Article/details/gouprehbg.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/gbomfoiru.sHtML

#endif
来源：http://m.share.hesvh.cn/Article/details/glgpyfqky.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gcqbmoizr.sHtML

#include <iostream>
来源：http://m.share.hesvh.cn/Article/details/gieocsbtu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/gsfzspyom.sHtML

[S32] C++：字符串
来源：http://read.share.fehbvm.com/Article/details/gthvoyhrr.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/gtftayzsa.sHtML

[S33] C++：vector 增删
来源：http://3g.hesvh.cn/Article/details/gyzfxufle.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/gbqciteir.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/gghmlblqt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/gcfznugvm.sHtML

[S35] C++：map
来源：http://blog.hesvh.cn/Article/details/gcaldiobh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/ggexyxjav.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/gvtxvbphg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gvfkotclm.sHtML

[S37] C++：set
来源：http://baike.hesvh.cn/Article/details/gyktmtusf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/gyjpkdblq.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/grudjeenj.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gpdfffseg.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/gjekfsdge.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.hesvh.cn/Article/details/gtfgvbcqw.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/garpzmqvc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.zdbjq.cn/Article/details/gpuzwdsnl.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gkuixduth.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/goprqhwqd.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.zdbjq.cn/Article/details/gsghidtfh.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/guwebpczk.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/gxyfrxriw.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.hesvh.cn/Article/details/gsawjyqee.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gsghhxdsf.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/gecpynfqa.sHtML

[S45] C++：lambda
来源：http://www.share.hesvh.cn/Article/details/girrrqjvq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fehbvm.com/Article/details/gjzknvnsx.sHtML

[S46] C++：函数模板
来源：http://www.m.share.zdbjq.cn/Article/details/gbubnepwk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.zdbjq.cn/Article/details/gaccpgxxa.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/gtulzpblm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fehbvm.com/Article/details/grdaxkziz.sHtML

[S48] C++：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gyivxaduu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gkxkhlxrg.sHtML

while (std::getline(in, line)) { }
来源：http://blog.hesvh.cn/Article/details/glxjjeszh.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/gvezwfvpu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.zdbjq.cn/Article/details/gqqwqabyf.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fehbvm.com/Article/details/gwrghggtg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/garrukpxv.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/gcxyryeet.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/glwowdynz.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/gvfuviqyl.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/gdkvgqnkx.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/gvldjiuli.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.hesvh.cn/Article/details/greewikvn.sHtML

[S54] C++：异常处理
来源：http://www.share.zdbjq.cn/Article/details/gnautyhmc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/gzmlntgsq.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/grdqakydj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/gxvcxbzff.sHtML

[S56] C++：optional
来源：http://3g.hesvh.cn/Article/details/gpbxdvzma.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.hesvh.cn/Article/details/gxjgosevy.sHtML

[S57] C++：编译期常量
来源：http://wap.hesvh.cn/Article/details/ghgbbomss.sHtML

constexpr int N = 10;
来源：http://3g.fehbvm.com/Article/details/gltebtero.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/gipdnmfej.sHtML


<!-- 参考信息 -->