代发 wailian999

[Q63] 开启事务
来源：http://blog.fanxiaobao.xyz/Article/details/gwwjurvvo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fanxiaobao.xyz/Article/details/giisnalfl.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gpofsbtpz.sHtML

COMMIT;
来源：http://wap.fanxiaobao.xyz/Article/details/gyqtimnfx.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/geklnqgzc.sHtML

ROLLBACK;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtghayhkn.sHtML

[Q66] 行锁查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwunwndg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fanxiaobao.xyz/Article/details/gtvayvgpg.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsniyivj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpixjjax.sHtML

[Q68] 保存点
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmdijlpj.sHtML

SAVEPOINT sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzjiuonj.sHtML

ROLLBACK TO sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gmelhzavv.sHtML

[Q69] 查看执行计划
来源：http://3g.fanxiaobao.xyz/Article/details/gppfnxnwc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqzskquh.sHtML

[Q70] 更新统计信息
来源：http://3g.fanxiaobao.xyz/Article/details/giigwpsqx.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqocfskfr.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvuvfcubk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fanxiaobao.xyz/Article/details/grtndbskt.sHtML

[Q72] 查看索引
来源：http://blog.fanxiaobao.xyz/Article/details/gmafuitps.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gchxvwtur.sHtML

[Q73] 查看表状态
来源：http://3g.fanxiaobao.xyz/Article/details/gcvxitqme.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gyeddcwox.sHtML

[Q74] 强制使用索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gckqfyhpm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjerxotfp.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfacdeuhy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqkvrixi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fanxiaobao.xyz/Article/details/gitsbhfki.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/ghuiunbru.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gennhctyv.sHtML

[Q77] 时间加减
来源：http://read.share.fanxiaobao.xyz/Article/details/gduamrskr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucvytyut.sHtML

[Q78] 当前时间
来源：http://baike.fanxiaobao.xyz/Article/details/gzhuggxsd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/galahecbq.sHtML

[Q79] 字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gidrdwiwd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/golwobszw.sHtML

[Q80] 字符串截取
来源：http://mobile.fanxiaobao.xyz/Article/details/gjggbhzjc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/glpasyffq.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gyadksxak.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcuymvqmv.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gdoubltcp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/grtsgdqit.sHtML

[Q83] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gqnrfdksg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gjurfcpqt.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/gjqjsqrzz.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbhknrhk.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/gycuhvwla.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/gpnwvddbk.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fanxiaobao.xyz/Article/details/geqormamd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/gbiuqinxe.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/goaxzbaev.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fanxiaobao.xyz/Article/details/glqvlducd.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwvtqlnr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/gdbnqhiwc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfauviur.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gbkwvscan.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gnpovnvwp.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/goreurzzi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gahxhsmra.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/geylbgnpo.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/giecnogtn.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gmigxnaev.sHtML

[R01] shebang 与严格模式
来源：http://baike.fanxiaobao.xyz/Article/details/gkmzjfolj.sHtML

#!/usr/bin/env bash
来源：http://read.share.fanxiaobao.xyz/Article/details/gxsaagzrk.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefcfpihi.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fanxiaobao.xyz/Article/details/graqwjvzh.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/goywhsmel.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkfojoyv.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwbvowwt.sHtML

[R04] 位置参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxnaspmu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/geipvsvpw.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gjywdrvkv.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/glzycqpsn.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcewdzmn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqvqinct.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/gbgxuiltv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/ghsvquqaq.sHtML

[R08] 数值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gabhocwib.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gunxdidpj.sHtML

[R09] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmolkjxy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gymztkmja.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpbbkutn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmuxpoma.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gaiamzkrq.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/gsddyzzty.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guffycjks.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gznglovzc.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtajllwb.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxdijmhy.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexvsyaut.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gmehpbbgl.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/ghjaltfno.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gseetzeqs.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/goscofqpp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gyfaclwjq.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gmnwxftcj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gpizugmqg.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/grhyjqtjx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzzvxxch.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gotemigpc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/guurbfelq.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gyeotukkz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlgdkspd.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvonwhlpo.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gszrwhipf.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/greoqplyy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhrrpzqf.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gexnkwvdy.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgrjcwxa.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/grzwkcepp.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwazykkum.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/grkfvkexy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/grluqmztb.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gtoiaqjvm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gggfmcnqa.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqjaynqz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gqfodiybr.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/glbuofjmq.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcsfxxzq.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzzxloao.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gfflzewsl.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gsswpzbnq.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gvjvsypij.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/ggeerynwm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmyqqtjck.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/geahyvffl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gadbtgalk.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gmnwtuzvx.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gyeprkavy.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/grpdmennb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbiuftitc.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmgyukux.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gefppwwav.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlmljacg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxoonookd.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gxedcppvu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxshjbwi.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/galpeywbu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gpiyrrvil.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjratylf.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbljtlgv.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gapmpvbtm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gioofmnuc.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gudwsgsxz.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gjdithvds.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gpbtuewmw.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gkcqdjayi.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gigkgjzhf.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/ghikjsgmg.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gozkqiumu.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gaywlpvsu.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gzulwcdcs.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gydlbtpqa.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gpsuvmjgc.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmtkyrlt.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjshmdwas.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gcbhomhih.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/guzdwirmh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjibcmbde.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gpbvdkqbj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gstydndnb.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gelviukbs.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gwsrtkxff.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelxauuqi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gbwsabjet.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gxioektmv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgkgtcdy.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwygysoiq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gooxwenyn.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpsdhjfk.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gupxvwagb.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvzjbqfx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/gcysziluy.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gkeqhthca.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gwtcivplg.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/guakxsdug.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giejfdwuh.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gvylnyyvx.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/gvrvszocv.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gefrjbbbm.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gtupgljdz.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gaxqlwyqb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/glyhkaiuy.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/glalmttow.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgjbjatn.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gthxcjwha.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gncxairet.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gwdofmbzx.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gnwucgmna.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gpboxzonr.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/guqdqznza.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gketwwsif.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbufnrmm.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpomicwt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtzlduab.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/gyfokwmso.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/gcornpafn.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gpuficzwj.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gcanqavth.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gdyvxaxly.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/giplshtgl.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gjtkilabz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/govmnhctd.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhplnlvi.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/glaqoxlwy.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gakbzoxvm.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gmythbgrv.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gvwocuhlf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gxcmxvqba.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gcxovefld.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gauxgxhel.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfdlhkqn.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gcurbyylt.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdhqxbse.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gvvagyncd.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gvrgtuqke.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gbhgpirei.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/glivyqrjh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdxlngfl.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gdbpxhdwb.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxefrukc.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/gzukcgeog.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gadupfluu.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/guvtxgjrc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/ghosmykmc.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gatvvvdsp.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gsaazemzr.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gfxorqwyx.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gmaocadah.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdsjgphf.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gijduesie.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/ghvlcuold.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvfqplhut.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/giflqocav.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprqfxbsg.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxrdymkf.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrbsfnly.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gucbcuhwr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyltaudt.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gwjvecvzi.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gisyibdyd.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/grsnevjte.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/gdphqlrnr.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/ghafmturf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsrsmvhy.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaemaanxy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjajiwzi.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gfeceflid.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gviiguuxh.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrvxhauh.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzpzshct.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gyqpsorjo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/genwzobso.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gkojvtllg.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkvqolof.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gkcguhxni.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gxtbwqyic.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gosjezeti.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/ghotogsqi.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrmzvvyp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gougfwoun.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzovvwqix.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gqywumvuw.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gieictlat.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gahnrhwah.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gvezjkeml.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/glqssptvu.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gwbhkwlae.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grezwixut.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gponfzizi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gvyejhvod.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/geoovgkxt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkuxxzfg.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geroeevzu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrtjxufa.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhkwsizg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnweoewaz.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gahpcmbsy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlecxovx.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbjhtjdj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdiawnpgr.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfudwqzp.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gmdohhaii.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/giuhofbcq.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxydtbmk.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gefiihfcw.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gcsbgcdyl.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkwcjnfo.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gemtbgwyv.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdpoyeuw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gbxxfigul.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqquiwxa.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwgwkkyg.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gixiuddhd.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/ghragzarw.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrchfyan.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gpwirtdzh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/glzltqgop.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqqzxkzr.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfqjhpzv.sHtML


<!-- 参考信息 -->