代发 wailian999

[Q67] 设置隔离级别
来源：http://m.share.fanxiaobao.xyz/Article/details/gygbmtpoo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnghytwlu.sHtML

[Q68] 保存点
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getbtniae.sHtML

SAVEPOINT sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gaddfkngb.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnhtfdhf.sHtML

[Q69] 查看执行计划
来源：http://3g.fanxiaobao.xyz/Article/details/gjqjbhrvr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fanxiaobao.xyz/Article/details/gmmnjscos.sHtML

[Q70] 更新统计信息
来源：http://3g.fanxiaobao.xyz/Article/details/ggwbjslde.sHtML

ANALYZE TABLE users;
来源：http://3g.fanxiaobao.xyz/Article/details/gfxruasgl.sHtML

[Q71] 查看建表语句
来源：http://baike.fanxiaobao.xyz/Article/details/gdrhljogx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fanxiaobao.xyz/Article/details/godmxydze.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbaaoizo.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymtencfx.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcfiddha.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gwggpuwuf.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/guknmfnzx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fanxiaobao.xyz/Article/details/gknamjwnb.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxebarcfe.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gejjrsuzb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/gkiuzqpev.sHtML

[Q76] 按天统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gcddvqjzc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/gfxbggnxn.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/gmtdbmycq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fanxiaobao.xyz/Article/details/gsidshrgs.sHtML

[Q78] 当前时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gdunljmnu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/gakqsjauz.sHtML

[Q79] 字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gflydefbq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrpxiwmu.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijslhnzo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvfzedsb.sHtML

[Q81] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvjpxzya.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgjvceif.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/gbmyykfst.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwuboaajf.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwtumizs.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvsiuvmf.sHtML

[Q84] 去除首尾空格
来源：http://3g.fanxiaobao.xyz/Article/details/guvkvcwaj.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gjujyvchm.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/gthlgrrms.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxihxxsno.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdbbgsix.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/gqvapczvp.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/gpjqqblyu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fanxiaobao.xyz/Article/details/glwesopur.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geishlthf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnyybzzc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrffyxmk.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/glatflpxe.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gmigwarrr.sHtML

[Q90] 生成序号列
来源：http://baike.fanxiaobao.xyz/Article/details/ghkgkemnv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/gyautechp.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmztmdhs.sHtML

R. Bash 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gplnvaxar.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnigcfik.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwbcwtqv.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/gofoathyt.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/gibrpsauo.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/gxqbxpdcq.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gjpdqkvwy.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gfeakieuq.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gxrmgbvmy.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gusvbhqsw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/giifhgcki.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlocuowc.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/geypwtnvm.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gtkosvbor.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtdyuayo.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/grhmtvqcb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcjphalo.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gkcumkesu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gxdrydswz.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gxripbtwt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gjutybynh.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhujuvpl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gpvfbarww.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gcskdwcgx.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/gnabniuqq.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gzdtpdjpl.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpafbgzc.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gmrdmijho.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gosmgruvg.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/glytstzvl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycuvtzwm.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/gdmxyfssv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gwpylnrqi.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdeyvcwbq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gcngmqobl.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gjgftryhl.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gxngysqab.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gcptapzys.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/glgxqqqgk.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gwyibsyoc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gicksjvgw.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvpgvyex.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gwcwjjpwx.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gtcbpwizm.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzuzylwmg.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gmuosduxi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gtejviuyn.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/guhosfqxl.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/glqbjuspl.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gfirwsftc.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gclyucurh.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwwucaby.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gamrrmrhq.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzjxwfkg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gcombvnun.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogoiwaav.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gfhkanhbq.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/ggobsdpvo.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gllpxohrl.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbcwggih.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfgpvtbs.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gnwyizcvl.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gbatkafaa.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gnfiqodxm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/glwvcoasm.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gthbrytic.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gdeprqxuu.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gnxxswwzd.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpttswiqt.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfchaebd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gcuwairrd.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/giegkpovu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gxjbqkvka.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/grbfrzqqa.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gqtsxowvs.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwsowbih.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/gztmyyoin.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/ggagdsgpt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzqckbgb.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gezdpkuxv.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gteqyglvi.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gbfeqarxr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gkazvbelf.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/guyhaxxer.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/grdespfix.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gghbmojcs.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnoryumx.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gdwqsfpbx.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxybtqnw.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/gbntaglpi.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/givffpdbq.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gnhbiqtop.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/ghocjgtzf.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gynybflfd.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gkrcfjghd.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gzzqbyrbg.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gpwodwfhz.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzyfccmha.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gngurfdkk.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gbwznhoen.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gsysmseek.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gkerbgmmo.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgcsoudh.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhybhiop.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvtcydhb.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gjluauufc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblwkxibd.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/goksdwrru.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gykcvbfrz.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gaufdtxjo.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnusaixi.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpjqgcyv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofyofjqp.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkhdiouv.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gbtaycmyl.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gonjxlwrl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhiaztgw.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthonyahq.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gfamakyay.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgvqdrbi.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxavlblu.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/goczhxcul.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gcmglstez.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gemwrivsm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsnnnjdt.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gizpqvggy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkortfmy.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvfjoyfx.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklazcnln.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhivtdpv.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gssubtcrv.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/geufrdetq.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvljsnot.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnoywrcks.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxgiotyo.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxbbhenx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/glxmqjmjs.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpagfmzp.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/gccwblwtp.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gizocgmtm.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/ghjilisyi.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbtjuxho.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhktjcjn.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gtuumemhn.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gakmsrhcf.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjlvriuf.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkaixjwxk.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxeemiwuw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/golbylxhi.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gsagdvtft.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/geezbisys.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gafeiwuih.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gyeltswhu.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/govqtzajx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtjvadvy.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gjazmczax.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpincknu.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmqvztib.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsrtxfuw.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxrqarwg.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gczqrrkqa.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/guollltjv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqwvyazc.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gobkihbjb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfstaanf.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxynhilik.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gnfiyuiqg.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ggszjbbgs.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gwnbwxecu.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmiihkdqp.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbaazzga.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gokaypcmw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxwnlvdm.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gzfmnfdty.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/glqpkafbp.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlbhsruw.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrgwndkm.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgcpgtli.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gjbdhpcqr.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genquwgla.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyurghhsy.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gnpothucr.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gnodjukbd.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxqsvnxr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdmzgyfg.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/glengkdkj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/gwnyclrvz.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gfewyjjzl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gbotxwsro.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxuwhosw.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gjjzggpse.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbmcidzl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gtudkpbkz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqwbwysu.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqkurssp.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gfhjdehjy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gaxpgulve.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/glpirohhy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrpzgtcb.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/glhedzfdu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gthfmihzi.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbnespnl.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdkniprv.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnuxywps.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gzytbqvck.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gmybtcgfo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjprpgmz.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gcgxiqmdb.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/genqelury.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrpebmsm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gihjrfagm.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gezwufokg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnfiuaal.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gyahtnuth.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorqlnubt.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gtabfevad.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpfpcauv.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqnekzoz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gwtlcpuyd.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gjjujvxfa.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gwadurxgs.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gzkdvozmb.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfyghyfsd.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmevhxid.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gekbtohcp.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gchgubept.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/galuphawg.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/guzfqhejh.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gnfgygvpt.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/giuwqfrqv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/grwbuetjh.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gckknygka.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gariyocgm.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjodwojc.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbtpklna.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsovwrvio.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gtxsnuhsx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqesgglnu.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glitogieo.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwwlspas.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gxcxgehst.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gsqrxpqey.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/gymkbclsl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdgxiwoun.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/galkvqmiu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhbodpqw.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gsymqpftl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhkffqhc.sHtML


<!-- 参考信息 -->