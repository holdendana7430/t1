代发 wailian999

[Q84] 去除首尾空格
来源：http://www.m.share.zdbjq.cn/Article/details/gztkwhwdx.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gwhpasiiu.sHtML

[Q85] 数值取整
来源：http://3g.hesvh.cn/Article/details/gcbusncyo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.zdbjq.cn/Article/details/gaylyxpfw.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.zdbjq.cn/Article/details/gqqnafiab.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/gqksemxif.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fehbvm.com/Article/details/gfyhsusyj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fehbvm.com/Article/details/gkghmwjco.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fehbvm.com/Article/details/gyyyfeunk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.hesvh.cn/Article/details/gtoircpto.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gbnxltqsp.sHtML

[Q89] 判断表是否存在
来源：http://3g.fehbvm.com/Article/details/gdfhowmdg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gczgbjktl.sHtML

[Q90] 生成序号列
来源：http://read.share.hesvh.cn/Article/details/gsilxegya.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fehbvm.com/Article/details/gsheinxfw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwlnowsps.sHtML

R. Bash 专题
来源：http://m.share.fehbvm.com/Article/details/ghmyhrnms.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghxsixutk.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/gqikoddhu.sHtML

#!/usr/bin/env bash
来源：http://m.share.zdbjq.cn/Article/details/guweqdeuh.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/ggzingxup.sHtML

[R02] 变量赋值与使用
来源：http://www.share.hesvh.cn/Article/details/gyerhratb.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/gfjnyjstd.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/grxsugiia.sHtML

readonly PI=3.14
来源：http://baike.hesvh.cn/Article/details/grdjuflxo.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/gdcfbcify.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.zdbjq.cn/Article/details/gkmyjktbs.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/gawzhazrc.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/gdilttgpn.sHtML

[R06] 判断命令是否存在
来源：http://3g.zdbjq.cn/Article/details/gvurasjar.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gytyaulix.sHtML

[R07] if 判断文件
来源：http://www.m.share.fehbvm.com/Article/details/gfecjbybw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/gqimnllzq.sHtML

[R08] 数值比较
来源：http://3g.zdbjq.cn/Article/details/giigccrpm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gclsfinae.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gmjszvpgj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gyghxxzfl.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/gdsjtzvpt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/gzdfikvkj.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/gualasjbb.sHtML

case "$1" in
来源：http://www.m.share.hesvh.cn/Article/details/gnahllbac.sHtML

start) echo "启动" ;;
来源：http://www.share.fehbvm.com/Article/details/gangfecrb.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/gzcgpjdkj.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/gqelqyosf.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/gjyqymrka.sHtML

[R12] for 遍历文件
来源：http://www.blog.fehbvm.com/Article/details/ggcpedocp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.zdbjq.cn/Article/details/gcvjbkkuy.sHtML

[R13] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/gzyxxqhzv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/ghcdbtwfc.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/giasculbf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gmavmhigu.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gzbtpfuhd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fehbvm.com/Article/details/glbkxlaik.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/guhehuzav.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gbtbznkez.sHtML

[R17] 数组定义与取值
来源：http://www.blog.zdbjq.cn/Article/details/gvyrlthna.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.hesvh.cn/Article/details/gvpvfjvoz.sHtML

[R18] 遍历数组
来源：http://www.blog.hesvh.cn/Article/details/gfntecmjy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/guspbujcg.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gznmgwmot.sHtML

echo "${#arr[@]}"
来源：http://www.blog.hesvh.cn/Article/details/gdaowmgso.sHtML

[R20] 关联数组（字典）
来源：http://baike.fehbvm.com/Article/details/giqqddagd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.zdbjq.cn/Article/details/gbgdxtrpc.sHtML

[R21] 字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gqyrbhyyk.sHtML

echo "${#s}"
来源：http://read.share.hesvh.cn/Article/details/gedhfcjhj.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/gvathgipl.sHtML

echo "${s:0:5}"
来源：http://mobile.zdbjq.cn/Article/details/gkitsddmz.sHtML

[R23] 字符串替换
来源：http://blog.hesvh.cn/Article/details/grdjrqzjm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.hesvh.cn/Article/details/gjqrjxnoo.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gpqtbbfaf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.zdbjq.cn/Article/details/glgmfdpbd.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/gbysnuodk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fehbvm.com/Article/details/gixvwmfnq.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/gyzykefrl.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.zdbjq.cn/Article/details/gynpmqbck.sHtML

[R27] 算术展开
来源：http://m.share.fehbvm.com/Article/details/gahvrxxnk.sHtML

echo $((1 + 2 * 3))
来源：http://3g.zdbjq.cn/Article/details/gqrhkbjug.sHtML

[R28] 浮点运算
来源：http://read.share.fehbvm.com/Article/details/gsxkxktgf.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/gqowowski.sHtML

[R29] 定义函数
来源：http://m.share.fehbvm.com/Article/details/grbncfbqh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/gmxsbrvle.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/gfmxlslmz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.hesvh.cn/Article/details/gcolczrbi.sHtML

[R31] 局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gsommotyv.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fehbvm.com/Article/details/gzaqxzxae.sHtML

[R32] 参数个数校验
来源：http://read.share.zdbjq.cn/Article/details/gppgyfcwm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gvabhbumn.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.zdbjq.cn/Article/details/gmladvkow.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/gvfncfelm.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/gpxzatcvv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gjtrehlfb.sHtML

[R35] 后台执行并等待
来源：http://wap.fehbvm.com/Article/details/gllbgsyef.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/gyobtzdhe.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/ghdnqpnqa.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/gcamzjpmi.sHtML

[R37] 把输出赋给变量
来源：http://baike.fehbvm.com/Article/details/guzvihfuu.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/ggpxrkywp.sHtML

[R38] 管道串联
来源：http://mobile.hesvh.cn/Article/details/gvsmhzkwz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.hesvh.cn/Article/details/gzkwrjipq.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/guipqwoha.sHtML

cmd > out.log 2>&1
来源：http://baike.fehbvm.com/Article/details/gtqgjqrns.sHtML

[R40] 追加写日志
来源：http://mobile.zdbjq.cn/Article/details/gsodezzgs.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/gopciswrl.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/gqpkamngy.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.zdbjq.cn/Article/details/guznpxzeb.sHtML

[R42] 输入重定向
来源：http://m.share.fehbvm.com/Article/details/gdrumzjfq.sHtML

wc -l < a.txt
来源：http://m.share.zdbjq.cn/Article/details/gfriapkhg.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/gdngbhfly.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/giunrxdgn.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/grjhjxeyw.sHtML

find . -mtime -7 -type f
来源：http://mobile.zdbjq.cn/Article/details/gfgcntgxk.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/gitedewik.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fehbvm.com/Article/details/glrhbownd.sHtML

[R46] 递归替换文件内容
来源：http://3g.hesvh.cn/Article/details/gzqctoolr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.zdbjq.cn/Article/details/gwgutlxjf.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/gelsomsfe.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/gxodkdvmc.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/gyysvzffp.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gmaekzbpj.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/gjrtdxvsf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.hesvh.cn/Article/details/gzvfiqczi.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/gszycbdhy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gmfadqwgc.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.hesvh.cn/Article/details/gjhmlpmga.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/gyfiivxmi.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/gmfswqqfd.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gmptuxrsm.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.zdbjq.cn/Article/details/gjdksoixb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fehbvm.com/Article/details/gyifabbep.sHtML

[R54] 比较两个文件
来源：http://blog.fehbvm.com/Article/details/gczbglgcd.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/gcdruluzj.sHtML

[R55] 压缩与解压
来源：http://wap.fehbvm.com/Article/details/gwffejdwo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/gqecltxlf.sHtML

[R56] 远程拷贝
来源：http://mobile.zdbjq.cn/Article/details/gmmswrmsf.sHtML

scp file user@host:/path/
来源：http://read.share.zdbjq.cn/Article/details/gagxachtw.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/ggeiyohmk.sHtML

ssh user@host 'uptime'
来源：http://www.blog.hesvh.cn/Article/details/gstweigiq.sHtML

[R58] 下载文件
来源：http://wap.hesvh.cn/Article/details/gehrzftzk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/gpzabmyjj.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gxowwlood.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/glwjnbtjf.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/ghzdhhgqc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/gvqlynrrf.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/gnoagbeeb.sHtML

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/gxqzwbahr.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/gujggbejp.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/gwlqjival.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gxjmjjvpb.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.zdbjq.cn/Article/details/gbhvslsof.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/giltatfqx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.zdbjq.cn/Article/details/gaujeeotu.sHtML

[R65] 查看端口占用
来源：http://m.share.zdbjq.cn/Article/details/gmnfjrkew.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.hesvh.cn/Article/details/gbairdgxi.sHtML

[R66] 定时任务
来源：http://www.blog.fehbvm.com/Article/details/gzwthyraf.sHtML

crontab -e;  crontab -l
来源：http://mobile.hesvh.cn/Article/details/gblsqbodh.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fehbvm.com/Article/details/gfysnimah.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/gksucokrk.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/gfmymdsss.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/gzkgzjqsl.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/gvaoxguof.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/gfcntncri.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/gvowputwc.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/gyxynyzmh.sHtML

[R71] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gypsvaqwl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/gnglbjcmz.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/gcnfhkkdp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gbxxmkwpt.sHtML

[R73] 分割大日志
来源：http://wap.hesvh.cn/Article/details/gkyvyvuyg.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/guwxvgauc.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/gqhirwsoe.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.zdbjq.cn/Article/details/guozrtlog.sHtML

[R75] 导出环境变量
来源：http://baike.hesvh.cn/Article/details/grflttqvz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.zdbjq.cn/Article/details/guopljlml.sHtML

[R76] 使用临时文件
来源：http://wap.fehbvm.com/Article/details/gnovcrrwa.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/ggzrsvfxo.sHtML

[R77] 读取用户输入
来源：http://3g.hesvh.cn/Article/details/gatqkfcch.sHtML

read -rp "请输入: " ans
来源：http://www.blog.hesvh.cn/Article/details/glwppfwpq.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/gllahynhb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.zdbjq.cn/Article/details/gkfebahhu.sHtML

[R79] 解析命令行选项
来源：http://3g.fehbvm.com/Article/details/gzgyatvzr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/gxtbqterp.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fehbvm.com/Article/details/gagkbqrqg.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/gapirzmld.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grnfzytky.sHtML

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/gvjjacwao.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkrjzebbm.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gxrkohpyq.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/gutgnwhgt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/gmltfktru.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/guidokmkp.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.zdbjq.cn/Article/details/gvsxldklw.sHtML

[S03] C：读入整数
来源：http://baike.zdbjq.cn/Article/details/grpqhslpe.sHtML

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/gffpkfxvf.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/gtidwlchd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gkiurfjwk.sHtML

[S05] C：字符串长度
来源：http://blog.fehbvm.com/Article/details/gqweqocle.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/gjzwmfswy.sHtML

[S06] C：字符串比较
来源：http://3g.zdbjq.cn/Article/details/gpjcbhdzk.sHtML

strcmp(a, b) == 0
来源：http://m.share.fehbvm.com/Article/details/gzjhurxfs.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/gzcoxiyxc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gxeduifnx.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/gcocwhtxc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fehbvm.com/Article/details/gixddducv.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fehbvm.com/Article/details/geknrytgg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/gbkyhnhdk.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/gabifjjva.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/gsguoximx.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/guvuhkwbi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/gsoxbuzxy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fehbvm.com/Article/details/gzagvgusk.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/gbvwqjsva.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/gsgewqtkz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/gswkldxlm.sHtML

[S13] C：宏定义
来源：http://3g.fehbvm.com/Article/details/gqvgeqpzq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/ghjixkvox.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/gfozeyqiw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.hesvh.cn/Article/details/gqynbowml.sHtML

[S15] C：类型转换
来源：http://3g.hesvh.cn/Article/details/ggjvmpsvb.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/gppisydco.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/giihmyusd.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/ghootjtih.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gtizerjaw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/gelnnczzx.sHtML

[S18] C：命令行参数
来源：http://wap.hesvh.cn/Article/details/gowllbfkw.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/gflcikvce.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/gfflbsntt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gvvvcholl.sHtML

[S20] C：二分查找
来源：http://m.share.zdbjq.cn/Article/details/gtjfldfby.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/grogjbqqs.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/ggbdihmjg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.zdbjq.cn/Article/details/gfecurmzg.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/gkxitzxkz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/gvuymzvxw.sHtML

[S23] C：随机数
来源：http://www.m.share.hesvh.cn/Article/details/gdzhksdlb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.hesvh.cn/Article/details/gwemnvduv.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/gfmdajrpj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.zdbjq.cn/Article/details/gqvcdbhqs.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/grbaykazp.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.zdbjq.cn/Article/details/gwecugxdd.sHtML

[S26] C：内存清零
来源：http://mobile.hesvh.cn/Article/details/ghyiswzfr.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gexadohym.sHtML

[S27] C：定义常量
来源：http://mobile.fehbvm.com/Article/details/gnujhjrxj.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gefwduyac.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/gikcggzow.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gzcltqwkv.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/gmhsqtnyi.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/gudmiupop.sHtML

[S30] C：头文件保护
来源：http://www.share.zdbjq.cn/Article/details/gnaolulww.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/gxnathrdg.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/gmgqcnzpe.sHtML

#endif
来源：http://m.share.hesvh.cn/Article/details/gqwbringa.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gdmwbfnin.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/gyxncguoy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/gjfrnngce.sHtML

[S32] C++：字符串
来源：http://www.share.hesvh.cn/Article/details/gdmmrpiiv.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/geapunxoo.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/gzsiujwbl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.hesvh.cn/Article/details/gucbellrc.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/gvylkptnf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/gfyjnnxia.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/glvbqicob.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gidvisfrj.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/gvadhcfvg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gjlzpauaf.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/goqrcvaqk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fehbvm.com/Article/details/golgmklsa.sHtML

[S38] C++：排序
来源：http://3g.zdbjq.cn/Article/details/ghfhiagak.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.hesvh.cn/Article/details/gkauiqqmt.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/gjsqfmzeu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/gxqdcekmt.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/ghudpynyf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.hesvh.cn/Article/details/gfqapvxjj.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/gkeayckpc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.hesvh.cn/Article/details/gjoylzsmj.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/gqjepnpix.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fehbvm.com/Article/details/gcgfkgura.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fehbvm.com/Article/details/gsvccckfb.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fehbvm.com/Article/details/gpbnnedpj.sHtML

[S44] C++：引用传参
来源：http://read.share.hesvh.cn/Article/details/gmibtqymt.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/gdahhqjdq.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/gxjjcalrc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.zdbjq.cn/Article/details/gcsnwgdnv.sHtML

[S46] C++：函数模板
来源：http://www.share.fehbvm.com/Article/details/gnrjethzq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gbfhofwvi.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/glilyobtq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.hesvh.cn/Article/details/gfhgxkyty.sHtML

[S48] C++：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gjbtsyoak.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/gaurnggpj.sHtML

while (std::getline(in, line)) { }
来源：http://blog.zdbjq.cn/Article/details/gfqmcfinv.sHtML

[S49] C++：写文件
来源：http://mobile.zdbjq.cn/Article/details/gzxuoiawr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/gfuudoame.sHtML

[S50] C++：格式化数字
来源：http://blog.zdbjq.cn/Article/details/gdjtbevws.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gkghaffrh.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fehbvm.com/Article/details/gadcdvpzn.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gzfsranwy.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.zdbjq.cn/Article/details/gwkvcjwwf.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fehbvm.com/Article/details/gzjpjrcey.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/gymsjkytt.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.hesvh.cn/Article/details/gbtuweril.sHtML

[S54] C++：异常处理
来源：http://wap.fehbvm.com/Article/details/gbzasjwnk.sHtML


<!-- 参考信息 -->