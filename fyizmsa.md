代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://wap.fehbvm.com/Article/details/gsmhdqvgy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fehbvm.com/Article/details/glugezbdq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.hesvh.cn/Article/details/gjieeazwp.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/ggwbpndex.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gfzbeiofz.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/gbfxkpoho.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/gfxrhnqge.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzppindzw.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/gsigiihhw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkfvqplsl.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/gpzohtdgg.sHtML

#!/usr/bin/env bash
来源：http://read.share.fehbvm.com/Article/details/gkdehjzda.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/grybynqdk.sHtML

[R02] 变量赋值与使用
来源：http://blog.zdbjq.cn/Article/details/guncgzscc.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fehbvm.com/Article/details/gwbuktafo.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/gnruibqnd.sHtML

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/gygvdnidt.sHtML

[R04] 位置参数
来源：http://baike.zdbjq.cn/Article/details/gjinnzjbl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.hesvh.cn/Article/details/ghfdhohup.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/gifdmchhi.sHtML

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/gqoiuwktt.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/gfhhenknr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gquuocdhi.sHtML

[R07] if 判断文件
来源：http://mobile.fehbvm.com/Article/details/gjimqwifl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/gwytqulpt.sHtML

[R08] 数值比较
来源：http://mobile.zdbjq.cn/Article/details/grjtvxqfb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.hesvh.cn/Article/details/giiccwutn.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gjuhpvqzd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fehbvm.com/Article/details/gqjtvaucw.sHtML

[R10] 正则匹配
来源：http://baike.fehbvm.com/Article/details/gagxgoyro.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fehbvm.com/Article/details/gehafbtem.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/ggsyzgcqt.sHtML

case "$1" in
来源：http://blog.hesvh.cn/Article/details/glzcggpqy.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gawzwhdiq.sHtML

stop)  echo "停止" ;;
来源：http://baike.hesvh.cn/Article/details/gznlecpls.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gtkpyzqyu.sHtML

esac
来源：http://m.share.fehbvm.com/Article/details/gqhtjwynj.sHtML

[R12] for 遍历文件
来源：http://www.blog.fehbvm.com/Article/details/ghyeypieo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/gnybcqkyv.sHtML

[R13] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/gahxhahxm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gcjdjjhkm.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/glqsmxxja.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gdtstuxjy.sHtML

[R15] while 逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gbfsfqcab.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fehbvm.com/Article/details/grnxnjneq.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/ghzeaconv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gvhbxkwrn.sHtML

[R17] 数组定义与取值
来源：http://www.blog.zdbjq.cn/Article/details/gwotrmvph.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.zdbjq.cn/Article/details/gmozvxyuw.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/gixavlbkp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gzsdwmtdi.sHtML

[R19] 数组长度
来源：http://3g.fehbvm.com/Article/details/gnxxymiap.sHtML

echo "${#arr[@]}"
来源：http://m.share.fehbvm.com/Article/details/gdmdbsobr.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fehbvm.com/Article/details/gzjofoqam.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/gzzmfgkwt.sHtML

[R21] 字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/grctxpnrh.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gcgrgrftr.sHtML

[R22] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/grfqfsbau.sHtML

echo "${s:0:5}"
来源：http://www.blog.hesvh.cn/Article/details/gelmtwtkk.sHtML

[R23] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/glaskpaup.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.hesvh.cn/Article/details/gtzbsikes.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gunrjdfsu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/glcmqjihc.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/ggcocvzru.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/gliosowvj.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/gjbmdjjjw.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.zdbjq.cn/Article/details/ghmzxfdjq.sHtML

[R27] 算术展开
来源：http://www.blog.fehbvm.com/Article/details/gilrybtxv.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.zdbjq.cn/Article/details/gcnlrvyqp.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/gjpvgmdpo.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.zdbjq.cn/Article/details/ggymmcqek.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/grekkmjqj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fehbvm.com/Article/details/gcwfqbvng.sHtML

[R30] 函数返回状态码
来源：http://read.share.hesvh.cn/Article/details/gpigsghqt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.hesvh.cn/Article/details/gknhpujck.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/gooeetlii.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.hesvh.cn/Article/details/gigjlafmh.sHtML

[R32] 参数个数校验
来源：http://m.share.zdbjq.cn/Article/details/gbshejotr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/geceknoxy.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.zdbjq.cn/Article/details/gnqcfsafd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.zdbjq.cn/Article/details/gcsuctrfi.sHtML

[R34] 退出时清理
来源：http://www.m.share.fehbvm.com/Article/details/giovqqqhv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gxugxscwc.sHtML

[R35] 后台执行并等待
来源：http://blog.hesvh.cn/Article/details/gzsrmzlsg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/ghsfwwatt.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.zdbjq.cn/Article/details/guylnvato.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fehbvm.com/Article/details/goxufqkgv.sHtML

[R37] 把输出赋给变量
来源：http://3g.fehbvm.com/Article/details/grklgpods.sHtML

files=$(ls -1)
来源：http://3g.zdbjq.cn/Article/details/gzyihfylb.sHtML

[R38] 管道串联
来源：http://read.share.fehbvm.com/Article/details/gnqcmakca.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/glfzvbafs.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.hesvh.cn/Article/details/gknhlrdqr.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/gqznluczl.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/gvopicnxr.sHtML

echo "log" >> out.log
来源：http://wap.fehbvm.com/Article/details/ghfkwzkhl.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/ggysgceai.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/gmhgvpljz.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/gfzviofky.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/gawvzxniy.sHtML

[R43] 按名字查找文件
来源：http://m.share.hesvh.cn/Article/details/gqvpbzebr.sHtML

find . -name "*.log" -type f
来源：http://www.share.fehbvm.com/Article/details/gmgcrktfz.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fehbvm.com/Article/details/gsirsyicn.sHtML

find . -mtime -7 -type f
来源：http://m.share.fehbvm.com/Article/details/gbiaqmzhp.sHtML

[R45] 批量删除
来源：http://blog.zdbjq.cn/Article/details/gnluecnxn.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fehbvm.com/Article/details/guluvoqqq.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gemwrugiu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fehbvm.com/Article/details/gzpltakni.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/ggpzwfdfx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.hesvh.cn/Article/details/gstidztnq.sHtML

[R48] awk 取指定列
来源：http://www.blog.hesvh.cn/Article/details/gijkcpkpr.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gwrvjeztn.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/gduuwnhrh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/gtmxqmfrn.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/gvqhkjfyh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/gexduwrvw.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/gtqizjgvg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fehbvm.com/Article/details/gtveocdkk.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/gcqitbrgr.sHtML

wc -l a.txt
来源：http://read.share.zdbjq.cn/Article/details/ghqiqmhhx.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/gwegwuztr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.zdbjq.cn/Article/details/gcjporkrd.sHtML

[R54] 比较两个文件
来源：http://www.m.share.hesvh.cn/Article/details/gsebaamrv.sHtML

diff a.txt b.txt
来源：http://3g.zdbjq.cn/Article/details/gxqkwanql.sHtML

[R55] 压缩与解压
来源：http://www.share.zdbjq.cn/Article/details/gjsolxuou.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.zdbjq.cn/Article/details/gcibxzqdi.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/gfuvcndjz.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/gmunjqayo.sHtML

[R57] 远程执行命令
来源：http://baike.zdbjq.cn/Article/details/gsvvyunus.sHtML

ssh user@host 'uptime'
来源：http://wap.fehbvm.com/Article/details/gylwcoikh.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/gynrjvygo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fehbvm.com/Article/details/gbtqyomjo.sHtML

[R59] 发 POST JSON
来源：http://3g.fehbvm.com/Article/details/gxzwwhqoz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.hesvh.cn/Article/details/gakvclquy.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gekcdykfv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/govxfaxai.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/gvdccynro.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/grixacmoa.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/gtgjecvpa.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/gccdflubk.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/gsppsosvj.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/gefqmzuzg.sHtML

[R64] 结束进程
来源：http://3g.zdbjq.cn/Article/details/gfxskbswi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/gyquptekz.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/gyssfshle.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/gnsxiolup.sHtML

[R66] 定时任务
来源：http://wap.hesvh.cn/Article/details/gihfutywk.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gfovhxthg.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/gqnphrnpg.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/guayakjkk.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/gqtxgwedy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gxbimkfvn.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/gjdervfux.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/glfbrzvak.sHtML

[R70] 时间戳与互转
来源：http://3g.zdbjq.cn/Article/details/grydvdumv.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gucousobo.sHtML

[R71] 日期格式化
来源：http://baike.hesvh.cn/Article/details/glezjqhrg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gnbisygui.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/gynlvdimg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gygqizymh.sHtML

[R73] 分割大日志
来源：http://www.blog.fehbvm.com/Article/details/gjyjosfps.sHtML

split -l 1000 big.log part_
来源：http://read.share.fehbvm.com/Article/details/gxcaxyqtt.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/glgskxvww.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.zdbjq.cn/Article/details/gzwepvbwr.sHtML

[R75] 导出环境变量
来源：http://3g.hesvh.cn/Article/details/gjjbaibqq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.hesvh.cn/Article/details/grefruiec.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/gaimqkaog.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gofciznvh.sHtML

[R77] 读取用户输入
来源：http://www.blog.fehbvm.com/Article/details/gkwvjaola.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.hesvh.cn/Article/details/gjusqcdrv.sHtML

[R78] 交互式菜单
来源：http://www.share.fehbvm.com/Article/details/gorlsvcwj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/gckckeggf.sHtML

[R79] 解析命令行选项
来源：http://3g.zdbjq.cn/Article/details/gzedtbatv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/gmvqjildq.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/gsmakuzha.sHtML

time ./run.sh
来源：http://wap.zdbjq.cn/Article/details/gvysvhkpw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbkihlowt.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/grbqwhbnj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggoerxkic.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/gekbcldfp.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/guaiukdpa.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/geqwttgou.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/gwzecwioz.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.zdbjq.cn/Article/details/gjakncgio.sHtML

[S03] C：读入整数
来源：http://baike.zdbjq.cn/Article/details/geewcqkvp.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/glzulfykr.sHtML

[S04] C：字符串复制
来源：http://mobile.hesvh.cn/Article/details/gadkkhpnj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/gfgxqokeg.sHtML

[S05] C：字符串长度
来源：http://blog.zdbjq.cn/Article/details/godfjtsxz.sHtML

strlen(s)
来源：http://m.share.fehbvm.com/Article/details/gntoiborh.sHtML

[S06] C：字符串比较
来源：http://www.blog.fehbvm.com/Article/details/guzhogdso.sHtML

strcmp(a, b) == 0
来源：http://wap.fehbvm.com/Article/details/gjzvyzahg.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/gzvpsnafu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/gscoghttc.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.hesvh.cn/Article/details/gvticdwdt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/gronugacs.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/gpizxiwii.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/ghajhrepc.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/gnbaakygi.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.hesvh.cn/Article/details/gvnshfxnz.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gqbfbyxri.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.hesvh.cn/Article/details/gixtxjmuo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gggqmqzjt.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gpqnrixwz.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/glheeitvl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/gcjkiopno.sHtML

[S13] C：宏定义
来源：http://mobile.hesvh.cn/Article/details/grtpukjfc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/glisggufe.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/gwedqmnpz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.hesvh.cn/Article/details/gqtidqgsx.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/geagblrwd.sHtML

(double) a / b
来源：http://www.blog.zdbjq.cn/Article/details/gjnwwlgva.sHtML

[S16] C：位操作置位
来源：http://read.share.fehbvm.com/Article/details/glkfsyvxf.sHtML

x |= (1 << 3);
来源：http://www.share.zdbjq.cn/Article/details/gozxokeqk.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/gtdknugto.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.zdbjq.cn/Article/details/gjrqwloqk.sHtML

[S18] C：命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gxnutjlup.sHtML

int main(int argc, char **argv)
来源：http://mobile.hesvh.cn/Article/details/ghdcqxnfn.sHtML

[S19] C：快速排序
来源：http://blog.zdbjq.cn/Article/details/gqzqhthpj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gfgrxonjo.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/gugjmqjum.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/ghlgueqzf.sHtML

[S21] C：字符类别判断
来源：http://blog.hesvh.cn/Article/details/gzbrywgil.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/ggmwtwldn.sHtML

[S22] C：字符串转数字
来源：http://www.share.hesvh.cn/Article/details/gstuhprip.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/gjbxsiiui.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/gprsebkua.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/guxxloykg.sHtML

[S24] C：获取本地时间
来源：http://wap.fehbvm.com/Article/details/gzxdnuefm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/gwiovdxky.sHtML

[S25] C：内存拷贝
来源：http://wap.zdbjq.cn/Article/details/gzcyzdfzq.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/grexempfz.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/gpcydghrk.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fehbvm.com/Article/details/ghjpzirsy.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gplscsvbb.sHtML

const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gxwljjqxq.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/gdcasggxi.sHtML

static int counter = 0;
来源：http://baike.zdbjq.cn/Article/details/gzsqnknyi.sHtML

[S29] C：变参函数
来源：http://3g.hesvh.cn/Article/details/gsegvbtdj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.hesvh.cn/Article/details/glhnzyshc.sHtML

[S30] C：头文件保护
来源：http://3g.fehbvm.com/Article/details/gkctsfqqq.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/gbkscijin.sHtML

#define X_H
来源：http://baike.hesvh.cn/Article/details/gpmjoqjxs.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/gthowkahc.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gqnjwcstv.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/gfjfseygl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fehbvm.com/Article/details/gzyahdhbz.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/gmjbroanz.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.hesvh.cn/Article/details/gpsqggfhk.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/gshdpfxhe.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fehbvm.com/Article/details/grsekxdcs.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/gqksuocew.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/gpcdaolyj.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/gljdqukzq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gvnplwttb.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/grdmvbuew.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/ghtlfyant.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/ggbsbvgcr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.zdbjq.cn/Article/details/ggogsxlud.sHtML

[S38] C++：排序
来源：http://www.blog.hesvh.cn/Article/details/gbhucyizp.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/grdgxmzro.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.hesvh.cn/Article/details/gydrkxxay.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/gjgldvvnp.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/gwzniyobm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.hesvh.cn/Article/details/gaotnpqti.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/gndtehmzi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/gfcragwju.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.hesvh.cn/Article/details/gupcgvncx.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/gxddtrgqi.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/geinnimvm.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/gjrgvpkma.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/gbqmrgsjx.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fehbvm.com/Article/details/gnpifqukg.sHtML

[S45] C++：lambda
来源：http://www.share.zdbjq.cn/Article/details/gkdvfejxa.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/gvoqgtlfh.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/gnagnmidj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/gsqpslrks.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/gkdyumywb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.zdbjq.cn/Article/details/gtpgwucny.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gjzdtnjgs.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/grrigxanp.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gkuisjpst.sHtML

[S49] C++：写文件
来源：http://www.share.zdbjq.cn/Article/details/gpiccqxxq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.zdbjq.cn/Article/details/gcgvtqlxi.sHtML

[S50] C++：格式化数字
来源：http://mobile.fehbvm.com/Article/details/gndrbwqho.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/geshrzdes.sHtML

[S51] C++：显式类型转换
来源：http://www.share.zdbjq.cn/Article/details/ggnhbqokr.sHtML

static_cast<double>(a) / b
来源：http://blog.hesvh.cn/Article/details/gfqimdfxh.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/gorofhclo.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fehbvm.com/Article/details/gtdlamots.sHtML

[S53] C++：移动语义
来源：http://read.share.fehbvm.com/Article/details/gccsvncyc.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/gdfmbjten.sHtML

[S54] C++：异常处理
来源：http://3g.fehbvm.com/Article/details/grqsnxcgh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/ggbfqclvo.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.hesvh.cn/Article/details/gbdmshing.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.hesvh.cn/Article/details/gdatxbxci.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/gzgaircvt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fehbvm.com/Article/details/gnpwipnjm.sHtML

[S57] C++：编译期常量
来源：http://3g.hesvh.cn/Article/details/gemqbbsml.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gvfqcwohy.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/gjhvuxtdc.sHtML


<!-- 参考信息 -->