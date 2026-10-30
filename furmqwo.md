代发 wailian999

[Q82] 字符长度与字节长度
来源：http://3g.fehbvm.com/Article/details/gquhccrwu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gsrtgdpyl.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/goamaqmgv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gotuhpmlj.sHtML

[Q84] 去除首尾空格
来源：http://3g.fehbvm.com/Article/details/gkuosvcnb.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gxwujlxny.sHtML

[Q85] 数值取整
来源：http://3g.hesvh.cn/Article/details/gliabwdkd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.hesvh.cn/Article/details/gtkhzwmch.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/gtaorkpmk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.zdbjq.cn/Article/details/gkxfraoxl.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.zdbjq.cn/Article/details/gpfdkasdy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fehbvm.com/Article/details/gpobfpxnb.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.zdbjq.cn/Article/details/gfgkbybqi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.hesvh.cn/Article/details/gaolwypew.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.hesvh.cn/Article/details/guswosilx.sHtML

[Q89] 判断表是否存在
来源：http://wap.hesvh.cn/Article/details/gbvwocfrn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gyngyziqb.sHtML

[Q90] 生成序号列
来源：http://wap.hesvh.cn/Article/details/gujornpgl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.zdbjq.cn/Article/details/gxretwyov.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gaccgugxe.sHtML

R. Bash 专题
来源：http://www.m.share.fehbvm.com/Article/details/gsoezwder.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/goupiplak.sHtML

[R01] shebang 与严格模式
来源：http://m.share.zdbjq.cn/Article/details/gpuhmqulu.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fehbvm.com/Article/details/gsayfwynt.sHtML

set -euo pipefail
来源：http://mobile.zdbjq.cn/Article/details/gjibpeguw.sHtML

[R02] 变量赋值与使用
来源：http://blog.zdbjq.cn/Article/details/ghyawknjy.sHtML

name="Tom"; echo "$name"
来源：http://wap.zdbjq.cn/Article/details/gqtmpeudz.sHtML

[R03] 只读变量
来源：http://www.blog.fehbvm.com/Article/details/gubaujniq.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/gzhoojayd.sHtML

[R04] 位置参数
来源：http://3g.hesvh.cn/Article/details/gngxdfipx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/ghtkmemaf.sHtML

[R05] 参数默认值
来源：http://read.share.fehbvm.com/Article/details/gklpskvsp.sHtML

name="${1:-default}"
来源：http://www.blog.fehbvm.com/Article/details/gtjexoipz.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fehbvm.com/Article/details/gfzhprtpm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gmwtrtgxd.sHtML

[R07] if 判断文件
来源：http://m.share.zdbjq.cn/Article/details/gblfgbzsx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/gwnbltyty.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/gscqknimz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.hesvh.cn/Article/details/gnuocyxsr.sHtML

[R09] 字符串比较
来源：http://wap.hesvh.cn/Article/details/gffemjdri.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.zdbjq.cn/Article/details/grbozxwxl.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/gdrxemrjj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.hesvh.cn/Article/details/guqvqgivh.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/gphtydemy.sHtML

case "$1" in
来源：http://www.m.share.zdbjq.cn/Article/details/gmcpveejf.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/gnvhnidtg.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fehbvm.com/Article/details/gvtittcok.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gucsysptl.sHtML

esac
来源：http://mobile.fehbvm.com/Article/details/gsvgnipxk.sHtML

[R12] for 遍历文件
来源：http://read.share.hesvh.cn/Article/details/gntlqzktg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/gklqrewvi.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/ghfvgxaky.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gfqmpahrq.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/gdrwphrcw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/ggxopblyt.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/giilstayb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.hesvh.cn/Article/details/ggtskmluv.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/gccpxtzoc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/glyjljkys.sHtML

[R17] 数组定义与取值
来源：http://3g.zdbjq.cn/Article/details/gnqlrehqm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.hesvh.cn/Article/details/gogghvvzg.sHtML

[R18] 遍历数组
来源：http://blog.zdbjq.cn/Article/details/gwdvxhssp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/gsfrgplad.sHtML

[R19] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gscthhsmh.sHtML

echo "${#arr[@]}"
来源：http://wap.hesvh.cn/Article/details/gjxhprrgv.sHtML

[R20] 关联数组（字典）
来源：http://blog.fehbvm.com/Article/details/gnfkdbvcy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/grjlpwggx.sHtML

[R21] 字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gdonlofhw.sHtML

echo "${#s}"
来源：http://read.share.hesvh.cn/Article/details/gaxjpjdcq.sHtML

[R22] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gvkqbltal.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/gsnrbkftl.sHtML

[R23] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gxgdljcid.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/gwlezrmmr.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gytbinjyu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/gkuhwoslv.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/gisygyymo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.zdbjq.cn/Article/details/gyxvekrbf.sHtML

[R26] 命令替换
来源：http://wap.zdbjq.cn/Article/details/gjlgrnhxa.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.zdbjq.cn/Article/details/gjflsikbc.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/gdxhvcups.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/gvhhtahvi.sHtML

[R28] 浮点运算
来源：http://m.share.hesvh.cn/Article/details/gbwwoxpvv.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.hesvh.cn/Article/details/gzkvrevzb.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gxygpvpmt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fehbvm.com/Article/details/gpusnbwjw.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/gwxgxwybt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fehbvm.com/Article/details/gcqomastr.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gcbddzexb.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.hesvh.cn/Article/details/gvrtveinr.sHtML

[R32] 参数个数校验
来源：http://m.share.hesvh.cn/Article/details/gnpjrjjcm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/genjouzci.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/gnbwbcxgu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fehbvm.com/Article/details/guspraaao.sHtML

[R34] 退出时清理
来源：http://wap.hesvh.cn/Article/details/gbkiihbff.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gxhrvnlgp.sHtML

[R35] 后台执行并等待
来源：http://www.share.hesvh.cn/Article/details/glgfyondj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.zdbjq.cn/Article/details/gojvqqitr.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/gfnvxkmio.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.zdbjq.cn/Article/details/gqozuqlrl.sHtML

[R37] 把输出赋给变量
来源：http://baike.fehbvm.com/Article/details/gsbomibkl.sHtML

files=$(ls -1)
来源：http://www.share.fehbvm.com/Article/details/gbkodrkyf.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/gixywmwnp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/gfhasoiwi.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.hesvh.cn/Article/details/gcxejlzyq.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/geeojeuyc.sHtML

[R40] 追加写日志
来源：http://3g.hesvh.cn/Article/details/grayljkil.sHtML

echo "log" >> out.log
来源：http://mobile.hesvh.cn/Article/details/gfbzpaxko.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/gggkzfsuj.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gtbyolmeh.sHtML

[R42] 输入重定向
来源：http://blog.fehbvm.com/Article/details/glwxafanq.sHtML

wc -l < a.txt
来源：http://wap.zdbjq.cn/Article/details/gsqwlcjzy.sHtML

[R43] 按名字查找文件
来源：http://blog.zdbjq.cn/Article/details/gxxkmldbq.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fehbvm.com/Article/details/grvcfpcdi.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/gdujxfajv.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/guciptrws.sHtML

[R45] 批量删除
来源：http://blog.fehbvm.com/Article/details/gmjpirsko.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.zdbjq.cn/Article/details/gicrfhgta.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/gkicsiwmv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/gdfvzilys.sHtML

[R47] sed 单行替换
来源：http://baike.hesvh.cn/Article/details/grvdiwhkh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fehbvm.com/Article/details/glgsrugpc.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/gvyrgylmv.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fehbvm.com/Article/details/gwjwinjlv.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/gdzmuvatw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.hesvh.cn/Article/details/gqpckxlkx.sHtML

[R50] awk 求和
来源：http://blog.fehbvm.com/Article/details/gfhtlqbkz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gfxklkxil.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/gbidrvhms.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fehbvm.com/Article/details/gtitdtlrj.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/gwbdtudat.sHtML

wc -l a.txt
来源：http://blog.zdbjq.cn/Article/details/gzwtsgkyf.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/guknmuotg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/gjbooquwy.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/ghpsqchvl.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/gkjnzyoxy.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/grbocqgcg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gtnvzxndk.sHtML

[R56] 远程拷贝
来源：http://3g.zdbjq.cn/Article/details/ghvmzicnu.sHtML

scp file user@host:/path/
来源：http://www.m.share.fehbvm.com/Article/details/gnurkbfcd.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/gxdkfthpb.sHtML

ssh user@host 'uptime'
来源：http://read.share.fehbvm.com/Article/details/gkpmnrhyo.sHtML

[R58] 下载文件
来源：http://wap.fehbvm.com/Article/details/gtfecmlje.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fehbvm.com/Article/details/gvdiowrcn.sHtML

[R59] 发 POST JSON
来源：http://m.share.fehbvm.com/Article/details/gcimuyfpj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fehbvm.com/Article/details/gfoeysumo.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gamkivkup.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.zdbjq.cn/Article/details/gqxhfaobg.sHtML

[R61] 磁盘占用
来源：http://baike.fehbvm.com/Article/details/galjhmell.sHtML

df -h;  du -sh *
来源：http://3g.fehbvm.com/Article/details/gckmvqbmg.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/gdsjadceo.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/gmgdbuxdz.sHtML

[R63] 内存与进程
来源：http://read.share.hesvh.cn/Article/details/gtixpolzq.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fehbvm.com/Article/details/geofvqcea.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gvbxlgflp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fehbvm.com/Article/details/gajicplvs.sHtML

[R65] 查看端口占用
来源：http://baike.fehbvm.com/Article/details/gvbauahxh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gyichqubo.sHtML

[R66] 定时任务
来源：http://www.share.fehbvm.com/Article/details/gujdlofqw.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/grggemmce.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/gtdptefab.sHtML

openssl rand -hex 16
来源：http://www.blog.hesvh.cn/Article/details/gdpukdvtd.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/gnjstpzkf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fehbvm.com/Article/details/gszovnvaf.sHtML

[R69] 生成随机密码
来源：http://www.share.hesvh.cn/Article/details/gkytszktq.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/geyrobqpz.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gjeutgvdx.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.zdbjq.cn/Article/details/gijdegogs.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gwynzvrzj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gwdqgjzdo.sHtML

[R72] 等待端口就绪
来源：http://m.share.fehbvm.com/Article/details/gxgpsetvu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/glljcpqqt.sHtML

[R73] 分割大日志
来源：http://www.blog.fehbvm.com/Article/details/gcuwoypxa.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/gtoqvhodv.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/gzximsxpg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fehbvm.com/Article/details/gjailehrx.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/gssrnxgsr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.zdbjq.cn/Article/details/glilhfubt.sHtML

[R76] 使用临时文件
来源：http://baike.hesvh.cn/Article/details/gyjpwuueg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/grqwtfvys.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/gbeiutpck.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/ggoidaczj.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/gkozijwua.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.zdbjq.cn/Article/details/gnpanftei.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/gginhprkt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/gdmmvtsei.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.hesvh.cn/Article/details/gpamxauoz.sHtML

time ./run.sh
来源：http://baike.zdbjq.cn/Article/details/gvrasfxwp.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdwzyejsm.sHtML

S. C / C++ 专题
来源：http://wap.hesvh.cn/Article/details/gnrjimrgm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gcrmvmhxt.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/gcwbfdkex.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/gwoxyfasc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/glyuqlhbq.sHtML

[S02] C：变量与格式化输出
来源：http://wap.zdbjq.cn/Article/details/gxyjnsjli.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.hesvh.cn/Article/details/gwjjylyex.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/gpiqrdbyc.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/gfpfumora.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/gaxnqnhnh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fehbvm.com/Article/details/gspekvgzn.sHtML

[S05] C：字符串长度
来源：http://baike.zdbjq.cn/Article/details/gkjradvce.sHtML

strlen(s)
来源：http://www.blog.zdbjq.cn/Article/details/gjdnghdgs.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gxlwjyfqj.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/gmnbvaiqb.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/gqbnatxpz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/gdlbjdesj.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/gijlvzqra.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/gmbutkyqq.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fehbvm.com/Article/details/ggstculbz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.hesvh.cn/Article/details/gtotmcyas.sHtML

[S10] C：指针与解引用
来源：http://m.share.fehbvm.com/Article/details/gmniszknw.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fehbvm.com/Article/details/gdoglqykp.sHtML

[S11] C：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gjnndpliw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.zdbjq.cn/Article/details/guwydtziz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.hesvh.cn/Article/details/gimvsggtt.sHtML

fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gzuxlcdma.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/grbodioji.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gptwjotbx.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/gntjopknr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/gcfmuzybr.sHtML

[S14] C：枚举
来源：http://blog.zdbjq.cn/Article/details/gjxkpfxlp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.hesvh.cn/Article/details/gmtahxmka.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/gpltdotxw.sHtML

(double) a / b
来源：http://read.share.hesvh.cn/Article/details/gikatvczu.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/gswzbakof.sHtML

x |= (1 << 3);
来源：http://3g.fehbvm.com/Article/details/gazonzcer.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gptkxoxca.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/gbrneasbw.sHtML

[S18] C：命令行参数
来源：http://read.share.fehbvm.com/Article/details/gksrmvruq.sHtML

int main(int argc, char **argv)
来源：http://mobile.fehbvm.com/Article/details/gcgnfgaxq.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/gtnyqsdjf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gdlculasd.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/gkvatyecy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gchlesntv.sHtML

[S21] C：字符类别判断
来源：http://read.share.fehbvm.com/Article/details/grgblusuo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/getggjzre.sHtML

[S22] C：字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gqprvldvs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/gpktmtdtw.sHtML

[S23] C：随机数
来源：http://mobile.hesvh.cn/Article/details/gbhaazpmk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/glmdesuzh.sHtML

[S24] C：获取本地时间
来源：http://www.share.hesvh.cn/Article/details/gcklvfudm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/gygyirpuw.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.hesvh.cn/Article/details/ggfmaljtw.sHtML

memcpy(dst, src, n);
来源：http://baike.hesvh.cn/Article/details/ggbbxxjuk.sHtML

[S26] C：内存清零
来源：http://baike.fehbvm.com/Article/details/gdxymnxmc.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fehbvm.com/Article/details/galsjueon.sHtML

[S27] C：定义常量
来源：http://mobile.fehbvm.com/Article/details/gbxnzayfv.sHtML

const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gbwficazi.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/gampocudi.sHtML

static int counter = 0;
来源：http://3g.fehbvm.com/Article/details/gsddabnrq.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/gziksljdc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fehbvm.com/Article/details/glygjjbsz.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/gakvexpys.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/gqvxomhfl.sHtML

#define X_H
来源：http://mobile.hesvh.cn/Article/details/gaddixztb.sHtML

#endif
来源：http://3g.zdbjq.cn/Article/details/gwygpppjr.sHtML

[S31] C++：Hello World
来源：http://wap.zdbjq.cn/Article/details/gtbkyecwf.sHtML

#include <iostream>
来源：http://wap.hesvh.cn/Article/details/gpbwzkyjy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/gncktuxty.sHtML

[S32] C++：字符串
来源：http://www.share.fehbvm.com/Article/details/gonqtikbd.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/gxhzmjvet.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/glsvklrum.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/gdrvijqqg.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/gozpyrzqw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/gjnfkhzra.sHtML

[S35] C++：map
来源：http://read.share.hesvh.cn/Article/details/gqqutzrij.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gqoqyztqx.sHtML

[S36] C++：unordered_map
来源：http://blog.fehbvm.com/Article/details/grtcdfgnp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gmhonnqnd.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/gwnwwfone.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fehbvm.com/Article/details/gwmygsucx.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/gvaxyxfin.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.hesvh.cn/Article/details/gpvwicrgd.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/gynpltswi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/gbdonpewu.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/gkkmulfup.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/gtxoflpju.sHtML

[S41] C++：类与构造函数
来源：http://m.share.zdbjq.cn/Article/details/gwbumlmsv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.hesvh.cn/Article/details/gyixkappb.sHtML

[S42] C++：继承与虚函数
来源：http://wap.hesvh.cn/Article/details/gcdfeipit.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/goihrzdcc.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/gkkemnpst.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/ggztfryji.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/gfgxozxwa.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fehbvm.com/Article/details/gkzvcgdxp.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/gojyjjzjn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.zdbjq.cn/Article/details/guwayeocb.sHtML

[S46] C++：函数模板
来源：http://www.share.fehbvm.com/Article/details/gqervzwzl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.hesvh.cn/Article/details/ggejlszth.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/grruvrvpl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fehbvm.com/Article/details/gkamaiosf.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gnuywqjlu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/gmmcqznch.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/gbjafkxqw.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/gmzczerfp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.hesvh.cn/Article/details/gfxtdkrme.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/gnkalhmou.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/gijwlcuum.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fehbvm.com/Article/details/gjqwtevwe.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/grirmnlgv.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/gpavyktmq.sHtML


<!-- 参考信息 -->