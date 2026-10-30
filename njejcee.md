代发 wailian999

[Q84] 去除首尾空格
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilyajzdq.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gaqgrlnoj.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/gflympukt.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwbuswpv.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fanxiaobao.xyz/Article/details/gydelqoty.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fanxiaobao.xyz/Article/details/gboseajdp.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/gsiktxjdi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdbexbxf.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlcwtmcm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fanxiaobao.xyz/Article/details/gzboxgtef.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gyepwxnrs.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwvhdzpr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gzrdmgxnx.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gmtijvoav.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtianbwsz.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gbtwyfbks.sHtML

R. Bash 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gxabdxhan.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gxbemhypg.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gpqvsihun.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/gljssudpy.sHtML

set -euo pipefail
来源：http://mobile.fanxiaobao.xyz/Article/details/gmybepzup.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmojfiais.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqfhniwu.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gixnczlhj.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmcrjduo.sHtML

[R04] 位置参数
来源：http://3g.fanxiaobao.xyz/Article/details/gptgqizio.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/gsvcnydqj.sHtML

[R05] 参数默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gghoxkgmr.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxfcctel.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gralikadx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gpxxlqhjc.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gourrrcyj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gqabdkuva.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/ggxxpycja.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdmeqhvu.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/goyrznwfn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gyawtkthe.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gwxdbfhtj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjshplnhs.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/griaccokh.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/guetcjpdf.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlwxgybu.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyubznmh.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gekbxkcbh.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gsmnulnwv.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/gypdsrdzs.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaquwqeba.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/groundyju.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtgvuumz.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/glyeqsywy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnrzqlih.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/grvtynoig.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gxijfvjzq.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcwonbip.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnyrgnby.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmquwdnmw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/guntznple.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gguqsfcpj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzwkejcn.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gcjsuuwte.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/glhsqvnuf.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gglqafnkj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gfephbpnv.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/ghthdeetk.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gykpgztzd.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtixymse.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpobthhk.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gpscoaxpx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/giwmbkfuj.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gtwkmuulj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbufyzixd.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvqlbfac.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdcadjxs.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/glbhesrzg.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gfydorxgm.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/gilzicqsv.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwjlnbdm.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdubzvevb.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwznvgnlw.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/gxcxvqrkk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmwvxflt.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdzmaxak.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdstludk.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gwmetljxm.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmcjbnjvt.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gqfcypnhl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcawjyvuc.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gnevjhavh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gqlkqxrdx.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gmcalqryk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gbtsejion.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gyqioieqh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzuvrtwrp.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfaxsveh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gtoeridri.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gtrxageug.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsofxjgi.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gyilamsgs.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gresxnmgb.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaocjdugw.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/glarcxwhw.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gxxovgfjs.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjqvvqnm.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gmwosgrep.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrvpxfme.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gufzkfdqn.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhtclipd.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkobjexb.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/giamxwyic.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gawhyeono.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjvekupz.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gevdroaxv.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/grkriozco.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghixjqthx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/ghjcwmacy.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyndywpbs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gsuudmang.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gromrymmn.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gylxqzoep.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gidjtwyfg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gtpmtjewm.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gairotpcu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gojsiyodk.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzaimhhzn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gulyepjoh.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvdbjsrt.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqwaoasb.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gitzyocva.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnlndbwb.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gqooxmmxt.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsiwgrgk.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gphziaiyb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/grwirpeue.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/ganbhbuec.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnoncevni.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/ghqragzdx.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/ggrsdyveb.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/goazcyhvy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gsoblalny.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmwutzyt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gbnuzrdjh.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnptsmkig.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfrhmjbp.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/ghrspetor.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqljoqgk.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gfssmjhfe.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gobncsnqy.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/glbkcainz.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfpzoero.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gtfxehrcz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxbdnvlq.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gimzmdkjl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gdqnzizsb.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbaleidc.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrzlxdzw.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizrnnfcx.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/gqclldwrw.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gbsrofbnt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gzuystlfk.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gmeadzeex.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdlslwde.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxnkgdux.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvdqhmkb.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gyadeajch.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gunnpoept.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gnumfmzme.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gajvvsene.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfgulhgo.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/ggiwklwta.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkyqfort.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhszyygd.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gapmdruie.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwbfxijf.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/grqnxqnki.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gkvlnswgc.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gbsuoehav.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/glegeegma.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/gqmqjnmwp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gkibxgwly.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gvdsxjedq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcprlpgq.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gsouoremp.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gmeivallp.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gyjbnetac.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkidautt.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwoovdvv.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gydbjhnxy.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gufoqfgvu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmtiopwt.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gjedrmnth.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gqdgeyrly.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gyedheyol.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gqrkntdbs.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjouzgvj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/goruclslv.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gybpqgyep.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsqtpqlq.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gtlvudmtf.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gopkyskes.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gzcbafagx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gottzatzq.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcuupriae.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/glcceumsu.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgnmesyv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gpzzdhkef.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gsvxomxgi.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfdwsujc.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gwoktqczg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gkkpjbzts.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghuvdptlh.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gfgiqqrgz.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gargmwhdg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdfcsviz.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfhcgzmj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlojelwd.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/guisenqgz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbnhwrbx.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzehvvngm.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gbzoscyrl.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gizbuioop.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmcuozph.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gplqvxrqf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtspbojkw.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/guirjuxfo.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gjegkcflp.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagogccla.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfdkctsw.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gmoxulmgj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwohmrpe.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/geylvkybs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gfiqenqvb.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gengdasbi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyacbluuv.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwoharagk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gbvodiajm.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gbctsfnzk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/glscwhofw.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewdorrrr.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/gisqfffqi.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbwzwgvb.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/gorgbjjpt.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/ghbsrcizu.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmueknffm.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtpksroh.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzqikglo.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gcntoqsev.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/ggylavhut.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjjosmfe.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gqwutemvl.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhcyexsg.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdcxckyn.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlfgngej.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsabpyvs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcbbhtxr.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/grwwvznjj.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gynsddzqc.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grozjtwvt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevwaexsx.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvhoatvp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/greyyipxi.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gykkmuvsj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gdvgvhfhb.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gnugubhlz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/givuobgoa.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvpuxval.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhlhwjjd.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/goveqgeip.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gtjsfadyn.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gcejkigjf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gotjaoqhx.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzudwatdd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsbgflme.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/grmbmwcoj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzndurcj.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbnwzeyv.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gflvfupqq.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/geuimeaad.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqopkrkm.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/ggyrvmnqb.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxgbpqfw.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomazguvb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gheudugxr.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gyolmlmlj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzpcmqvgl.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxoxrmwy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gohwbbvux.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgzvaosl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbuphdear.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gxqhmswul.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkqjtldh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gztouyvab.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/guumfywkm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gbvrhhupr.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxpjstwh.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/gqnqwixvh.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbnczhxp.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfriobhj.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/gqoqtmqef.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gynbscbsv.sHtML

[S54] C++：异常处理
来源：http://wap.fanxiaobao.xyz/Article/details/gnwgkhoaq.sHtML


<!-- 参考信息 -->