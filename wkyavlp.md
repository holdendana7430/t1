代发 wailian999

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/gfeeurald.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gjpwepnet.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gmoruqxxx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/glapmillv.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/guwuaqwbm.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gxmrimcmk.sHtML

[Q85] 数值取整
来源：http://baike.zdbjq.cn/Article/details/goniezwnr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.hesvh.cn/Article/details/gvqxzwwmu.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fehbvm.com/Article/details/goywvjydk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.zdbjq.cn/Article/details/gokospxth.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fehbvm.com/Article/details/gelllgxmc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.hesvh.cn/Article/details/gjdclnlqo.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.hesvh.cn/Article/details/gnwocsqyi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fehbvm.com/Article/details/ghgvpbpsx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/gepvrpvea.sHtML

[Q89] 判断表是否存在
来源：http://mobile.hesvh.cn/Article/details/guwtcbate.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.hesvh.cn/Article/details/gjysabnbr.sHtML

[Q90] 生成序号列
来源：http://www.share.zdbjq.cn/Article/details/gxersksjg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.hesvh.cn/Article/details/gscbfzqbj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkqqpzclb.sHtML

R. Bash 专题
来源：http://wap.fehbvm.com/Article/details/guwzobiec.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gcqzoqrwh.sHtML

[R01] shebang 与严格模式
来源：http://blog.zdbjq.cn/Article/details/giifgwznb.sHtML

#!/usr/bin/env bash
来源：http://mobile.fehbvm.com/Article/details/gtrjogvwu.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/glchkzfxg.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/giyxfsoox.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fehbvm.com/Article/details/gvnuzqmli.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/gaufbqyhh.sHtML

readonly PI=3.14
来源：http://www.share.fehbvm.com/Article/details/gidjqftmt.sHtML

[R04] 位置参数
来源：http://read.share.zdbjq.cn/Article/details/gxzzwcilt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.hesvh.cn/Article/details/gygyzjrfr.sHtML

[R05] 参数默认值
来源：http://mobile.zdbjq.cn/Article/details/ggakdqgqv.sHtML

name="${1:-default}"
来源：http://wap.hesvh.cn/Article/details/glrkhvhxv.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/gbjpxxamr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gicjpzjiq.sHtML

[R07] if 判断文件
来源：http://m.share.zdbjq.cn/Article/details/gqsdinpit.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/gttyrulmz.sHtML

[R08] 数值比较
来源：http://wap.fehbvm.com/Article/details/gajdrkzcs.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/grwiknwtr.sHtML

[R09] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/gqpvtqsbk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/gqlazhwqm.sHtML

[R10] 正则匹配
来源：http://blog.fehbvm.com/Article/details/grfcwfxhl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.zdbjq.cn/Article/details/glxysqtsq.sHtML

[R11] case 多分支
来源：http://m.share.fehbvm.com/Article/details/gmhqenzql.sHtML

case "$1" in
来源：http://wap.zdbjq.cn/Article/details/gexbkureo.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/gnzlakskr.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gkeegggfy.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/gsqudloee.sHtML

esac
来源：http://www.share.zdbjq.cn/Article/details/gebzwbfyg.sHtML

[R12] for 遍历文件
来源：http://m.share.zdbjq.cn/Article/details/gelemxbcs.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/gogcjjatj.sHtML

[R13] for 计数循环
来源：http://3g.hesvh.cn/Article/details/gtudnoody.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gzmjrbsqk.sHtML

[R14] C 风格 for
来源：http://www.share.zdbjq.cn/Article/details/gxfqiawcc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gwxupqjqn.sHtML

[R15] while 逐行读文件
来源：http://baike.hesvh.cn/Article/details/gwcphgsud.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/gjymtbxkx.sHtML

[R16] until 等待条件
来源：http://baike.hesvh.cn/Article/details/gfunbbpyz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gnfefewrj.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/gccpipvfx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fehbvm.com/Article/details/gichqtwiz.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/glmcrijms.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.zdbjq.cn/Article/details/gyffzohlq.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gfkiysulc.sHtML

echo "${#arr[@]}"
来源：http://mobile.hesvh.cn/Article/details/gruoldrwj.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.zdbjq.cn/Article/details/gtlvvsohp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/ghymuyzxo.sHtML

[R21] 字符串长度
来源：http://www.share.fehbvm.com/Article/details/gnwzqpyum.sHtML

echo "${#s}"
来源：http://www.m.share.zdbjq.cn/Article/details/gvcxlfgaw.sHtML

[R22] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/guqbqtbgg.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/gdnzjguhn.sHtML

[R23] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gieggsqrp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/gnesiflxq.sHtML

[R24] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gohcwsfrz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/govkxdwbd.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fehbvm.com/Article/details/gbopzmjkw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fehbvm.com/Article/details/gvfxbbdpz.sHtML

[R26] 命令替换
来源：http://mobile.fehbvm.com/Article/details/ghwfbpklr.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.hesvh.cn/Article/details/gctaleccg.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/gsytryqkc.sHtML

echo $((1 + 2 * 3))
来源：http://blog.hesvh.cn/Article/details/gczvlkajm.sHtML

[R28] 浮点运算
来源：http://baike.fehbvm.com/Article/details/gqlcisqnr.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.zdbjq.cn/Article/details/gptunumzc.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gkhxztmpq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/gftrohgso.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/gngztubsd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fehbvm.com/Article/details/gcmmumtub.sHtML

[R31] 局部变量
来源：http://www.blog.hesvh.cn/Article/details/gwidvfumm.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/gkppbtspx.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/gnppwygfl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gqkybqzep.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.hesvh.cn/Article/details/gjbhamjjo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fehbvm.com/Article/details/glfsxagnq.sHtML

[R34] 退出时清理
来源：http://read.share.fehbvm.com/Article/details/gxkcwhnbu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gwljaktqd.sHtML

[R35] 后台执行并等待
来源：http://wap.zdbjq.cn/Article/details/gbrzthpqm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.zdbjq.cn/Article/details/gobfdhtol.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/gtfchwiyf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.hesvh.cn/Article/details/ghqxyblji.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/gvzqocins.sHtML

files=$(ls -1)
来源：http://www.share.hesvh.cn/Article/details/gdjqnjdwb.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/gclvmlqoa.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.zdbjq.cn/Article/details/gribdltht.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/ghiykwrhv.sHtML

cmd > out.log 2>&1
来源：http://blog.hesvh.cn/Article/details/gffsbyzjx.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/gpoogvcnp.sHtML

echo "log" >> out.log
来源：http://read.share.hesvh.cn/Article/details/ghnwngfuf.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/gcrdejlom.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/giueylbjn.sHtML

[R42] 输入重定向
来源：http://wap.fehbvm.com/Article/details/glwowtzim.sHtML

wc -l < a.txt
来源：http://read.share.hesvh.cn/Article/details/gcntqsnvc.sHtML

[R43] 按名字查找文件
来源：http://www.blog.hesvh.cn/Article/details/gkervrdey.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/ggmobalkm.sHtML

[R44] 按修改时间查找
来源：http://3g.hesvh.cn/Article/details/gwelmzxlr.sHtML

find . -mtime -7 -type f
来源：http://wap.zdbjq.cn/Article/details/goxoqvwnq.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/gykdnhmxi.sHtML

find . -name "*.tmp" -delete
来源：http://wap.hesvh.cn/Article/details/gqudnczqx.sHtML

[R46] 递归替换文件内容
来源：http://blog.fehbvm.com/Article/details/gsvlmquyi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.zdbjq.cn/Article/details/gtontmyop.sHtML

[R47] sed 单行替换
来源：http://baike.zdbjq.cn/Article/details/gfgxbgsbm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/gjcpphhif.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/gznxhojeu.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gthdwsyyv.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gjaplnlrl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.zdbjq.cn/Article/details/grtycmdnb.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/gpdnvzkkf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gbitdqiei.sHtML

[R51] 排序去重取前几
来源：http://www.share.zdbjq.cn/Article/details/gfdofytdk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gdopqydfh.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/gkixpnwsi.sHtML

wc -l a.txt
来源：http://m.share.hesvh.cn/Article/details/gpokfugud.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.hesvh.cn/Article/details/ggjtnfhcv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.zdbjq.cn/Article/details/ghthyjcwo.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/gzmcaoiib.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/gshtuhdkk.sHtML

[R55] 压缩与解压
来源：http://wap.zdbjq.cn/Article/details/gbzwgklhr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fehbvm.com/Article/details/gliqkedrk.sHtML

[R56] 远程拷贝
来源：http://3g.fehbvm.com/Article/details/gehurlxeq.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/gpejbuuoo.sHtML

[R57] 远程执行命令
来源：http://mobile.zdbjq.cn/Article/details/gggirtnqy.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/gvrobkwgb.sHtML

[R58] 下载文件
来源：http://wap.hesvh.cn/Article/details/glyvhybaf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.zdbjq.cn/Article/details/guafeacui.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gilxbllsk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.zdbjq.cn/Article/details/gmymmuyiu.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/grtgztocj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.zdbjq.cn/Article/details/gpwgqcitl.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/gmlmmvqyr.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/gzekssxna.sHtML

[R62] 找最占空间的文件
来源：http://blog.hesvh.cn/Article/details/gpsguguog.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.hesvh.cn/Article/details/gpmrokyus.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/giqxhkcmo.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fehbvm.com/Article/details/gsbdwavkl.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/gfrcowynw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gtyectejc.sHtML

[R65] 查看端口占用
来源：http://m.share.hesvh.cn/Article/details/gzmrbjeud.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.zdbjq.cn/Article/details/gzjqiangr.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gobmlldfd.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/gupqqiizc.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/gvntpgqgq.sHtML

openssl rand -hex 16
来源：http://www.blog.hesvh.cn/Article/details/gosnggsaf.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/gddlxevlc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.hesvh.cn/Article/details/gbyzbqmfe.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/gzvmxiihp.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.zdbjq.cn/Article/details/gpwixvfzr.sHtML

[R70] 时间戳与互转
来源：http://3g.fehbvm.com/Article/details/gqxintwci.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/gvjhzpddz.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/goeefkybo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gxdxxeeyp.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/gnnpdefna.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gbnqosudr.sHtML

[R73] 分割大日志
来源：http://www.m.share.hesvh.cn/Article/details/girnojbpj.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fehbvm.com/Article/details/gfmsbiqhr.sHtML

[R74] 批量重命名
来源：http://www.m.share.fehbvm.com/Article/details/gpcxrhtlh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.zdbjq.cn/Article/details/gdumbnpis.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/gbhthgksx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.hesvh.cn/Article/details/gmepmiuwk.sHtML

[R76] 使用临时文件
来源：http://wap.zdbjq.cn/Article/details/gajlbygcj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/geuwbcolg.sHtML

[R77] 读取用户输入
来源：http://baike.zdbjq.cn/Article/details/gymtqodlt.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/gfraekpmm.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/gmynfqiqs.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/gtuvvqrxc.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/gpxquiqmy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fehbvm.com/Article/details/gdijjxdtl.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.zdbjq.cn/Article/details/gbgbtfshz.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/ghejgroye.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gzaiszdim.sHtML

S. C / C++ 专题
来源：http://baike.hesvh.cn/Article/details/gbekjtnjr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gylaervkz.sHtML

[S01] C：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gimqifxdo.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/glopogkvi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.hesvh.cn/Article/details/goaeozhtx.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gwnpavuci.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/gtadmioaa.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/ghwzigazm.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/gwaiedrlc.sHtML

[S04] C：字符串复制
来源：http://www.blog.zdbjq.cn/Article/details/gyfhskjgy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gkwjnmmin.sHtML

[S05] C：字符串长度
来源：http://wap.zdbjq.cn/Article/details/gemarklke.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/grrvosopu.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/gexkbvzwu.sHtML

strcmp(a, b) == 0
来源：http://m.share.zdbjq.cn/Article/details/ggryyuzhj.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/ginerxfdj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/gatiteajn.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/guxrwbokt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/gzcvasujx.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.zdbjq.cn/Article/details/goiyxxcaj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.hesvh.cn/Article/details/gunhidzkm.sHtML

[S10] C：指针与解引用
来源：http://m.share.zdbjq.cn/Article/details/glapkgwpx.sHtML

int *p = &a;  *p = 5;
来源：http://baike.zdbjq.cn/Article/details/gyipucncc.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gzmgisffo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/gjdafjdts.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fehbvm.com/Article/details/gpsdxadnn.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/goibtbkcj.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/gcvrpahre.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.hesvh.cn/Article/details/gyfmtivgf.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/gzhjebhdh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.zdbjq.cn/Article/details/gkyxubbzi.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/glkfwkege.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.hesvh.cn/Article/details/gxyfsahrr.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/gzlytsqhg.sHtML

(double) a / b
来源：http://blog.zdbjq.cn/Article/details/gzvhdimmh.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/gwkoxdrzp.sHtML

x |= (1 << 3);
来源：http://www.blog.hesvh.cn/Article/details/gwotzfkpx.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.hesvh.cn/Article/details/ghjvamggx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.zdbjq.cn/Article/details/gymkhlvpy.sHtML

[S18] C：命令行参数
来源：http://m.share.hesvh.cn/Article/details/grfyirhng.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/gckzlmyqc.sHtML

[S19] C：快速排序
来源：http://www.share.fehbvm.com/Article/details/gcpkusffj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gesbraavx.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/gmggzesas.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/geumifaro.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/gukilapxm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/guqamtgxn.sHtML

[S22] C：字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gvjwcmikx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fehbvm.com/Article/details/gfzqhsvwm.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/giobhuawk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/gvhjqqzzj.sHtML

[S24] C：获取本地时间
来源：http://blog.zdbjq.cn/Article/details/ggwfgglin.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gsnvjyndz.sHtML

[S25] C：内存拷贝
来源：http://mobile.fehbvm.com/Article/details/gfrkldykj.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/gyghfrgwz.sHtML

[S26] C：内存清零
来源：http://m.share.fehbvm.com/Article/details/gysevahqv.sHtML

memset(a, 0, sizeof a);
来源：http://wap.hesvh.cn/Article/details/gwobxzekm.sHtML

[S27] C：定义常量
来源：http://blog.zdbjq.cn/Article/details/gzkircyhi.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gesruvolj.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/gxmqnlunm.sHtML

static int counter = 0;
来源：http://baike.zdbjq.cn/Article/details/gknspzaff.sHtML

[S29] C：变参函数
来源：http://mobile.fehbvm.com/Article/details/gfsqqxazy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.zdbjq.cn/Article/details/ggzkousmc.sHtML

[S30] C：头文件保护
来源：http://read.share.hesvh.cn/Article/details/gsxdrspoa.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/gkvumaqna.sHtML

#define X_H
来源：http://www.m.share.fehbvm.com/Article/details/gbaiwhfxx.sHtML

#endif
来源：http://www.m.share.zdbjq.cn/Article/details/gkfmiianc.sHtML

[S31] C++：Hello World
来源：http://blog.zdbjq.cn/Article/details/godofhlse.sHtML

#include <iostream>
来源：http://m.share.hesvh.cn/Article/details/glxsducpk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/gfeyupwlu.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/gtsteluth.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/glafcghlq.sHtML

[S33] C++：vector 增删
来源：http://3g.hesvh.cn/Article/details/gfdbmeegm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/gkmtcdqsp.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/gunhqvvie.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/gliptblsy.sHtML

[S35] C++：map
来源：http://www.share.hesvh.cn/Article/details/ggrkgfjmh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gfcvjwniu.sHtML

[S36] C++：unordered_map
来源：http://wap.hesvh.cn/Article/details/gbtfccvaw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gcrvxotrh.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/gcvahbgth.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/gpjoukexp.sHtML

[S38] C++：排序
来源：http://3g.hesvh.cn/Article/details/gvvmtmjkt.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/giyimmqpt.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fehbvm.com/Article/details/gbbzcirhl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fehbvm.com/Article/details/glryckhzh.sHtML

[S40] C++：查找元素
来源：http://www.share.hesvh.cn/Article/details/gbnwtlmuv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/gqjkbpjud.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/gspivtsdi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.hesvh.cn/Article/details/ggrxoxltd.sHtML

[S42] C++：继承与虚函数
来源：http://wap.hesvh.cn/Article/details/gabjbrhxf.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fehbvm.com/Article/details/gncxyjbhp.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/gxhzhokfh.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.zdbjq.cn/Article/details/goqjeanug.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/gtzqgqxov.sHtML

void inc(int &x) { ++x; }
来源：http://wap.zdbjq.cn/Article/details/gtpczynzy.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/gmnzynkrp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/gpiqvtgzi.sHtML

[S46] C++：函数模板
来源：http://blog.fehbvm.com/Article/details/gxwteasrs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.zdbjq.cn/Article/details/gvbqzoxqo.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/gykgntlua.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.hesvh.cn/Article/details/gnkzfhxhu.sHtML

[S48] C++：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gddaxgyoc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.hesvh.cn/Article/details/gbqvyrzyc.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fehbvm.com/Article/details/ghvlzlcdt.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/gzbbyvksq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gtsolxlto.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.hesvh.cn/Article/details/ghntkhfta.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gxnvydbhl.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/grduzjrgi.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.hesvh.cn/Article/details/ggneubvmz.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.hesvh.cn/Article/details/gedvicjtl.sHtML


<!-- 参考信息 -->