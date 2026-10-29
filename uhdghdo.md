代发 wailian999

[Q78] 当前时间
来源：http://3g.hesvh.cn/Article/details/grenqjodw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.zdbjq.cn/Article/details/guwiokbdq.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/gcxfvcznz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.zdbjq.cn/Article/details/gpntchmuk.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/godfclfou.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.hesvh.cn/Article/details/geyumoxow.sHtML

[Q81] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/ghwqflqac.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/ghhekqlya.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fehbvm.com/Article/details/ghpfrgbnv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gnpkbquiy.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gktknlyuc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/greowmsrd.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/gmjmqqkkk.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gjpavyzeq.sHtML

[Q85] 数值取整
来源：http://baike.zdbjq.cn/Article/details/gfddopcxx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fehbvm.com/Article/details/gjstrdnsb.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.hesvh.cn/Article/details/gspuehukn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fehbvm.com/Article/details/gbitnhwjg.sHtML

[Q87] JSON 字段做条件
来源：http://3g.hesvh.cn/Article/details/gatvxoilo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.zdbjq.cn/Article/details/gfxkhbvzp.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.zdbjq.cn/Article/details/gyawjtaga.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.zdbjq.cn/Article/details/gjfjyofrv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/ghamjmabk.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/glscoesjh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.zdbjq.cn/Article/details/gvztgacvx.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/gnbolatre.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fehbvm.com/Article/details/gdzbepyxo.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqwjdzvcs.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/gnstacmle.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqzizbexh.sHtML

[R01] shebang 与严格模式
来源：http://baike.fehbvm.com/Article/details/gxzmhwjbb.sHtML

#!/usr/bin/env bash
来源：http://3g.hesvh.cn/Article/details/gntpuwmir.sHtML

set -euo pipefail
来源：http://wap.hesvh.cn/Article/details/gqcdbvxpc.sHtML

[R02] 变量赋值与使用
来源：http://m.share.hesvh.cn/Article/details/gidudawna.sHtML

name="Tom"; echo "$name"
来源：http://wap.hesvh.cn/Article/details/gsszkkizo.sHtML

[R03] 只读变量
来源：http://m.share.zdbjq.cn/Article/details/ghrtjcozi.sHtML

readonly PI=3.14
来源：http://baike.fehbvm.com/Article/details/girbrdacg.sHtML

[R04] 位置参数
来源：http://www.blog.hesvh.cn/Article/details/gbjkrzxti.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/goiuidjry.sHtML

[R05] 参数默认值
来源：http://read.share.fehbvm.com/Article/details/giulhnxxh.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/gmxhpyhju.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gaxooqnsg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gognxdnfm.sHtML

[R07] if 判断文件
来源：http://read.share.hesvh.cn/Article/details/gzqniogxy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fehbvm.com/Article/details/groohkzsh.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/gpnpqjxbh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.hesvh.cn/Article/details/gsturegfy.sHtML

[R09] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/giazfmeep.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fehbvm.com/Article/details/geoorlcaw.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/gyqrlvpeg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.hesvh.cn/Article/details/glpcemcwq.sHtML

[R11] case 多分支
来源：http://www.m.share.fehbvm.com/Article/details/ghddknfio.sHtML

case "$1" in
来源：http://www.m.share.fehbvm.com/Article/details/gtknwncqi.sHtML

start) echo "启动" ;;
来源：http://wap.hesvh.cn/Article/details/gdohkionc.sHtML

stop)  echo "停止" ;;
来源：http://wap.fehbvm.com/Article/details/glhoeksuw.sHtML

*)     echo "未知命令" ;;
来源：http://wap.hesvh.cn/Article/details/gseshpioo.sHtML

esac
来源：http://read.share.hesvh.cn/Article/details/gjdctsahe.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/gzcmedfeo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.hesvh.cn/Article/details/gnuwopueu.sHtML

[R13] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/gihamvfbo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gshncxvpf.sHtML

[R14] C 风格 for
来源：http://baike.hesvh.cn/Article/details/gnjtsdygm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/ghacyczzd.sHtML

[R15] while 逐行读文件
来源：http://wap.hesvh.cn/Article/details/guqqpudas.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.hesvh.cn/Article/details/gellwfymf.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/gzwfllbdu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gsnpaxtyf.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fehbvm.com/Article/details/garxscjtw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.hesvh.cn/Article/details/geawnlbdk.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/ggemtmyge.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.zdbjq.cn/Article/details/gufuiafvn.sHtML

[R19] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gbuqmildb.sHtML

echo "${#arr[@]}"
来源：http://read.share.hesvh.cn/Article/details/gmcfnjogn.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.hesvh.cn/Article/details/gmacqtkyn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.hesvh.cn/Article/details/gjktjifxz.sHtML

[R21] 字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gyjusdggq.sHtML

echo "${#s}"
来源：http://www.m.share.zdbjq.cn/Article/details/grccxlrlb.sHtML

[R22] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gktutoozm.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/grhncmarh.sHtML

[R23] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gnwnaruvt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fehbvm.com/Article/details/gyajwqhlu.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gluqscwli.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fehbvm.com/Article/details/ghxuhezji.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/gismfthyk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/gajsgngqd.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/gdblyxsvs.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.zdbjq.cn/Article/details/gmbrixwhw.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/gkmeuvddj.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.hesvh.cn/Article/details/ghxmihdpb.sHtML

[R28] 浮点运算
来源：http://mobile.zdbjq.cn/Article/details/gizfinjxb.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/gtdviqwrc.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/gstryfvai.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/gajqxqjvc.sHtML

[R30] 函数返回状态码
来源：http://www.blog.zdbjq.cn/Article/details/ggpkhqbdh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/guvoavbpr.sHtML

[R31] 局部变量
来源：http://www.m.share.hesvh.cn/Article/details/geetsgvfj.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.hesvh.cn/Article/details/grqaxlpvx.sHtML

[R32] 参数个数校验
来源：http://read.share.zdbjq.cn/Article/details/gxeblgukd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/ghcjnydot.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/gggnccrpw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/ggzqjofgu.sHtML

[R34] 退出时清理
来源：http://www.blog.zdbjq.cn/Article/details/gpmoxnehq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gtftsjnui.sHtML

[R35] 后台执行并等待
来源：http://www.share.hesvh.cn/Article/details/gppsfyyxr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.zdbjq.cn/Article/details/gefvwmbro.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fehbvm.com/Article/details/gzroczjug.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.zdbjq.cn/Article/details/gvkwynuqh.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.hesvh.cn/Article/details/gcjycqrth.sHtML

files=$(ls -1)
来源：http://www.blog.fehbvm.com/Article/details/gufrecdyr.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/ggvsqyryn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.hesvh.cn/Article/details/gjqskkirk.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.hesvh.cn/Article/details/gyxwtckqs.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/ggsjwdgeq.sHtML

[R40] 追加写日志
来源：http://3g.hesvh.cn/Article/details/gvwpqncdw.sHtML

echo "log" >> out.log
来源：http://wap.zdbjq.cn/Article/details/gzlavgcif.sHtML

[R41] 丢弃输出
来源：http://baike.fehbvm.com/Article/details/gkmtqagvg.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fehbvm.com/Article/details/gdfrltnxe.sHtML

[R42] 输入重定向
来源：http://blog.zdbjq.cn/Article/details/ggpyvxlon.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/gburkrkxz.sHtML

[R43] 按名字查找文件
来源：http://baike.fehbvm.com/Article/details/gkqqilqxq.sHtML

find . -name "*.log" -type f
来源：http://www.blog.hesvh.cn/Article/details/gsanxlqtm.sHtML

[R44] 按修改时间查找
来源：http://mobile.fehbvm.com/Article/details/ghdogrihc.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/ggkopuonx.sHtML

[R45] 批量删除
来源：http://m.share.zdbjq.cn/Article/details/gqvrzmuxq.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gcneeiiwi.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fehbvm.com/Article/details/geezmtfsu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.hesvh.cn/Article/details/ghtgafxwa.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/ggrheuddi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.zdbjq.cn/Article/details/ghvapocib.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/gzqfyhbfp.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fehbvm.com/Article/details/guasziwny.sHtML

[R49] awk 带条件
来源：http://mobile.zdbjq.cn/Article/details/gchzohamd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gswiufwuf.sHtML

[R50] awk 求和
来源：http://3g.hesvh.cn/Article/details/gsfvpelzo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/gxptdhxzs.sHtML

[R51] 排序去重取前几
来源：http://www.blog.hesvh.cn/Article/details/gbprohigt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.hesvh.cn/Article/details/gmdoivqhq.sHtML

[R52] 统计行数
来源：http://read.share.hesvh.cn/Article/details/gnfmzmudc.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gcfmgsmoq.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/ghdypcymw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fehbvm.com/Article/details/gaqcnulov.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/goycsgsnh.sHtML

diff a.txt b.txt
来源：http://3g.fehbvm.com/Article/details/gmngcrkos.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/gurqydgat.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gsmlksxqu.sHtML

[R56] 远程拷贝
来源：http://baike.hesvh.cn/Article/details/gisyqbftr.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/gqytmoehh.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/gbinomxex.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/gqkdrwhuh.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/ggcpoatoe.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/gbwkrppqr.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/gjwnocwqm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fehbvm.com/Article/details/gwiibftyv.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gmxxyrbfz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.hesvh.cn/Article/details/gdyxjnmwb.sHtML

[R61] 磁盘占用
来源：http://read.share.zdbjq.cn/Article/details/guwmhlifg.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/gwsuxdzti.sHtML

[R62] 找最占空间的文件
来源：http://m.share.zdbjq.cn/Article/details/gjkrdadbl.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.hesvh.cn/Article/details/gaxqhjemg.sHtML

[R63] 内存与进程
来源：http://www.m.share.hesvh.cn/Article/details/gmbxccavi.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/ghhkcpyzo.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/gqoqaaisq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.zdbjq.cn/Article/details/guahpfzun.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/gshfpgnkj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/gncapmdiy.sHtML

[R66] 定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gdurkoxjm.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/goebyfswa.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/gccapilak.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/gftwlyevr.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fehbvm.com/Article/details/gfrelnuum.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/gsqrpqblt.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/gsnyheuvd.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/gflkciwdc.sHtML

[R70] 时间戳与互转
来源：http://blog.zdbjq.cn/Article/details/gregiqgsb.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/gmxbevlfa.sHtML

[R71] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gigbjzpdd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gdmtgokdp.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/gyfswoehy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gkapvcegp.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/gwcvgrfxn.sHtML

split -l 1000 big.log part_
来源：http://www.share.zdbjq.cn/Article/details/gdsuvzbgq.sHtML

[R74] 批量重命名
来源：http://wap.fehbvm.com/Article/details/gspkealzk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gsqrplfdp.sHtML

[R75] 导出环境变量
来源：http://blog.hesvh.cn/Article/details/gwohnylba.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.zdbjq.cn/Article/details/guzppwvhp.sHtML

[R76] 使用临时文件
来源：http://baike.hesvh.cn/Article/details/ggvhbgxpy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gbpzejokn.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/gpihxqtnw.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.hesvh.cn/Article/details/gemhutsin.sHtML

[R78] 交互式菜单
来源：http://wap.zdbjq.cn/Article/details/ghwdpyxlh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/gqhydwtwo.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/gaczzkcal.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fehbvm.com/Article/details/gvyocjrfj.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gtjumopuk.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/gispypxdi.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/guvazgmib.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/gjzazacof.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glsrbsfal.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/guqcamana.sHtML

#include <stdio.h>
来源：http://www.m.share.fehbvm.com/Article/details/geookxgcr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.hesvh.cn/Article/details/gkwcwyxoq.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gfemnixsc.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fehbvm.com/Article/details/gauphlzhk.sHtML

[S03] C：读入整数
来源：http://mobile.fehbvm.com/Article/details/gyqhfgrzf.sHtML

int x; scanf("%d", &x);
来源：http://mobile.hesvh.cn/Article/details/gquppobwr.sHtML

[S04] C：字符串复制
来源：http://3g.hesvh.cn/Article/details/guudmxioq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.hesvh.cn/Article/details/gnipczwcw.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/gcrlfocno.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/gahyuoegw.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/gfyehukkp.sHtML

strcmp(a, b) == 0
来源：http://read.share.zdbjq.cn/Article/details/gnesunqln.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/gapzwxhqj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.hesvh.cn/Article/details/gowvhuepk.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/giwdfefgl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.zdbjq.cn/Article/details/gtarpjpgw.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/ghvcszyhz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/ghpnwcyid.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/gnhdqwrmv.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.hesvh.cn/Article/details/gsazbxgut.sHtML

[S11] C：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gjawinexb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.hesvh.cn/Article/details/gnzldwxfk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fehbvm.com/Article/details/ghotffvhn.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gulledjnl.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gpxdrpyof.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gzvekihqg.sHtML

[S13] C：宏定义
来源：http://www.share.zdbjq.cn/Article/details/gwvevqpba.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.hesvh.cn/Article/details/gqhxgfyqd.sHtML

[S14] C：枚举
来源：http://3g.hesvh.cn/Article/details/gafikqigk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.hesvh.cn/Article/details/giiyrpcaf.sHtML

[S15] C：类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gpdjzjxyv.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gmxgfixer.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/gchaqrprj.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/gisuphjjf.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gxwbrziie.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/galehvvtm.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/gnlpwcnad.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/gqtintmqe.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/glmwhfmpi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gzpibypxv.sHtML

[S20] C：二分查找
来源：http://wap.hesvh.cn/Article/details/gnsngsohe.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gatfssuwq.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fehbvm.com/Article/details/gaodzhdsa.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fehbvm.com/Article/details/gttwglcvm.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/ggtdmqmza.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.zdbjq.cn/Article/details/gydbunkup.sHtML

[S23] C：随机数
来源：http://m.share.zdbjq.cn/Article/details/glltmjosh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/gqhavlaku.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/gsmvzymqn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/gncfbhpug.sHtML

[S25] C：内存拷贝
来源：http://mobile.hesvh.cn/Article/details/gjewxifei.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/gbpseivhm.sHtML

[S26] C：内存清零
来源：http://baike.hesvh.cn/Article/details/gvxcjiurr.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/ggsowpxew.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/gdusnjbds.sHtML

const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gyeadacmp.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/gvualrmap.sHtML

static int counter = 0;
来源：http://3g.hesvh.cn/Article/details/gyoktkmas.sHtML

[S29] C：变参函数
来源：http://mobile.fehbvm.com/Article/details/gtkiaovmt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/gjavwajya.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/geureqked.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/gmiiuiiyv.sHtML

#define X_H
来源：http://www.m.share.fehbvm.com/Article/details/gcwxnivqq.sHtML

#endif
来源：http://blog.hesvh.cn/Article/details/gpslfsffx.sHtML

[S31] C++：Hello World
来源：http://blog.hesvh.cn/Article/details/gpjmxbjrz.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/gujznxwxq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/gnbzeywdd.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/gzbfprdui.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/gnfiuevpj.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/gbrfalqpf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fehbvm.com/Article/details/grenjqxbb.sHtML

[S34] C++：遍历 vector
来源：http://3g.hesvh.cn/Article/details/gnxrebcbr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/gdfhhvxjo.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/gvehzetwl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gtfgbpzpf.sHtML

[S36] C++：unordered_map
来源：http://mobile.zdbjq.cn/Article/details/grdikrydq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/geoxgvgks.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/gnhlgeeot.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/gffzfzeab.sHtML

[S38] C++：排序
来源：http://wap.zdbjq.cn/Article/details/gjvtcxzrp.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/gqkkqtonj.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.zdbjq.cn/Article/details/gpqraxjhf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/gdbrignbj.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/gnxytayuh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/gqwujgekl.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gdedgdplb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/grwyuxzsi.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/gwcowztxe.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/gwipwsjfb.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/gkmaxjbai.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.hesvh.cn/Article/details/gwnwgimju.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/gvcvjmcwd.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/gafkyyxhl.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/giegjkbbs.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/gkuzrvbmz.sHtML

[S46] C++：函数模板
来源：http://read.share.fehbvm.com/Article/details/gmgkdinjp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/glezkfqba.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/gnbjmtygo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/glrpplxsc.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gxkxvlzjt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fehbvm.com/Article/details/ghgzgyarf.sHtML


<!-- 参考信息 -->