代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.zdbjq.cn/Article/details/gziluvsse.sHtML

[Q52] 删除指定行
来源：http://baike.zdbjq.cn/Article/details/gozdgqqzk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gmdufuwya.sHtML

[Q53] 按条件删除
来源：http://read.share.zdbjq.cn/Article/details/gnmvulixh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.hesvh.cn/Article/details/gffhnkpfz.sHtML

[Q54] 清空表
来源：http://3g.zdbjq.cn/Article/details/gpvebrthx.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.zdbjq.cn/Article/details/gkdclrxjy.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.hesvh.cn/Article/details/gxobzhfnw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gpvsqtlnc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/glqcopmwx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gtkkwrntq.sHtML

[Q57] 行号
来源：http://m.share.fehbvm.com/Article/details/gbyonuisj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.hesvh.cn/Article/details/gitmlqmiq.sHtML

[Q58] 累计求和
来源：http://baike.fehbvm.com/Article/details/gkkmkdchq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gewkdpqjl.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/gkzugjxoy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gtcdenihz.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.zdbjq.cn/Article/details/gtliwglun.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.hesvh.cn/Article/details/gyztulprj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gefmcqetn.sHtML

[Q61] 移动平均
来源：http://blog.zdbjq.cn/Article/details/gauwrehmx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gblysonzb.sHtML

[Q62] 分组占比
来源：http://mobile.hesvh.cn/Article/details/gbzubbcxz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gqtdtpdbo.sHtML

[Q63] 开启事务
来源：http://m.share.hesvh.cn/Article/details/gnygyjvms.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.hesvh.cn/Article/details/gfrgbpike.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/gfxiccxan.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/gwwnkhdgg.sHtML

[Q65] 回滚事务
来源：http://blog.hesvh.cn/Article/details/gyptqleek.sHtML

ROLLBACK;
来源：http://m.share.zdbjq.cn/Article/details/gidawgmbz.sHtML

[Q66] 行锁查询
来源：http://3g.hesvh.cn/Article/details/gfjmntqti.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.zdbjq.cn/Article/details/gvhqtyfxc.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.hesvh.cn/Article/details/gqobxfzkj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fehbvm.com/Article/details/ggxugtzny.sHtML

[Q68] 保存点
来源：http://wap.fehbvm.com/Article/details/gnxwcajuv.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gmjcznvoi.sHtML

ROLLBACK TO sp1;
来源：http://blog.hesvh.cn/Article/details/gwvpmbyhj.sHtML

[Q69] 查看执行计划
来源：http://www.share.hesvh.cn/Article/details/ggrsipjyl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/gyasowhhn.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/grzfpaqyg.sHtML

ANALYZE TABLE users;
来源：http://mobile.hesvh.cn/Article/details/guoejgpqn.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/gpjsnmvur.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/gdclgdvqu.sHtML

[Q72] 查看索引
来源：http://3g.zdbjq.cn/Article/details/gtqgicjws.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/gorjkqlcv.sHtML

[Q73] 查看表状态
来源：http://read.share.zdbjq.cn/Article/details/gndfblifm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.hesvh.cn/Article/details/gjqjixclr.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fehbvm.com/Article/details/gwxgcpzfa.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fehbvm.com/Article/details/ghqxqovap.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/glpdiylsn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gzomgotfs.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.zdbjq.cn/Article/details/gegodcpko.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/gvqyubafc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.zdbjq.cn/Article/details/glwpqdhnv.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/gcgyyvvlj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fehbvm.com/Article/details/geszuqnoi.sHtML

[Q78] 当前时间
来源：http://www.blog.zdbjq.cn/Article/details/gyxbrjnnc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.zdbjq.cn/Article/details/gjdkfkdtq.sHtML

[Q79] 字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gumkfwjhq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.hesvh.cn/Article/details/gvpzjzctc.sHtML

[Q80] 字符串截取
来源：http://www.share.fehbvm.com/Article/details/gcvirpqno.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gznfpfadn.sHtML

[Q81] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gmoayohye.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gffkuwojd.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.zdbjq.cn/Article/details/gohbgmksh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gtwthzmma.sHtML

[Q83] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gizlavlbl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/grmldijlk.sHtML

[Q84] 去除首尾空格
来源：http://baike.zdbjq.cn/Article/details/gbiioqmjh.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gfxlxgtyr.sHtML

[Q85] 数值取整
来源：http://3g.zdbjq.cn/Article/details/gcnfkszym.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.zdbjq.cn/Article/details/gtdrgtrtz.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.zdbjq.cn/Article/details/gvzznaxum.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.zdbjq.cn/Article/details/gcdtxkqpz.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.hesvh.cn/Article/details/gpxmpsfhr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fehbvm.com/Article/details/gdmgurkqb.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/gqetvqylf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.zdbjq.cn/Article/details/ggwiuvybf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.zdbjq.cn/Article/details/gkccskjse.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gafzbijik.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.zdbjq.cn/Article/details/gatatdgir.sHtML

[Q90] 生成序号列
来源：http://3g.zdbjq.cn/Article/details/grhhvmelk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fehbvm.com/Article/details/gymgdnpdx.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtvekjsoc.sHtML

R. Bash 专题
来源：http://wap.zdbjq.cn/Article/details/ghedryyqq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtrioyejj.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/gkntlecwa.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/gulvudqpx.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/gxvhxuoic.sHtML

[R02] 变量赋值与使用
来源：http://www.share.hesvh.cn/Article/details/gcuneexan.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.zdbjq.cn/Article/details/geajskkac.sHtML

[R03] 只读变量
来源：http://blog.fehbvm.com/Article/details/gzjobyzkx.sHtML

readonly PI=3.14
来源：http://read.share.zdbjq.cn/Article/details/gyqjjuees.sHtML

[R04] 位置参数
来源：http://blog.zdbjq.cn/Article/details/gusbyekkn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/gqxdbvbnp.sHtML

[R05] 参数默认值
来源：http://3g.fehbvm.com/Article/details/gwegbjsau.sHtML

name="${1:-default}"
来源：http://m.share.hesvh.cn/Article/details/gwvabzghw.sHtML

[R06] 判断命令是否存在
来源：http://www.share.zdbjq.cn/Article/details/ghxohsrcv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gqcpijvsx.sHtML

[R07] if 判断文件
来源：http://mobile.hesvh.cn/Article/details/gfjrjhtgo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.hesvh.cn/Article/details/gzqvglmwb.sHtML

[R08] 数值比较
来源：http://mobile.fehbvm.com/Article/details/gipzbykre.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.zdbjq.cn/Article/details/gjrgjrrrj.sHtML

[R09] 字符串比较
来源：http://baike.fehbvm.com/Article/details/gjyndyydp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/gijfsxqig.sHtML

[R10] 正则匹配
来源：http://www.share.zdbjq.cn/Article/details/glblmvorn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/gkhzmtpvm.sHtML

[R11] case 多分支
来源：http://wap.fehbvm.com/Article/details/gesvgovub.sHtML

case "$1" in
来源：http://baike.zdbjq.cn/Article/details/ghlabqqyj.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/gbwddpzsp.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/gmrwelios.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/goxzqvlea.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/ggimhhbal.sHtML

[R12] for 遍历文件
来源：http://www.share.zdbjq.cn/Article/details/guwdgygik.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.hesvh.cn/Article/details/gkecbtmtn.sHtML

[R13] for 计数循环
来源：http://3g.hesvh.cn/Article/details/gjilqmlui.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/grvjahraw.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/gfanocenj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gzzlqjuaw.sHtML

[R15] while 逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gobuzdwbt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/gpgoewdmu.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/gsdqohbvj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gjeyilhba.sHtML

[R17] 数组定义与取值
来源：http://blog.zdbjq.cn/Article/details/gzdjngadi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/gbuzttyfb.sHtML

[R18] 遍历数组
来源：http://3g.fehbvm.com/Article/details/ggtlrzvsb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/gsuacwoyp.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gaqvwacva.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gusjdkjco.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fehbvm.com/Article/details/glewurbri.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.hesvh.cn/Article/details/gmpqelssk.sHtML

[R21] 字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gulltyihb.sHtML

echo "${#s}"
来源：http://3g.zdbjq.cn/Article/details/ghywfnxgg.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/gxhmluvse.sHtML

echo "${s:0:5}"
来源：http://mobile.zdbjq.cn/Article/details/gmzmoqcaw.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gjcmlfpbr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/gaamvyjry.sHtML

[R24] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/ghftamggj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/glzlwbuug.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.zdbjq.cn/Article/details/gyjqydcoc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fehbvm.com/Article/details/grcagioag.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/gfbfrerne.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.zdbjq.cn/Article/details/glmcrglru.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/gmnwhirpr.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/gezudunbq.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/gikboxhwy.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fehbvm.com/Article/details/gfgzkwelu.sHtML

[R29] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/grpjqkpvq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.hesvh.cn/Article/details/giiogpxez.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/gcbnpefoe.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.hesvh.cn/Article/details/gqrofrwws.sHtML

[R31] 局部变量
来源：http://mobile.hesvh.cn/Article/details/garlsauzo.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fehbvm.com/Article/details/goxkclesw.sHtML

[R32] 参数个数校验
来源：http://m.share.hesvh.cn/Article/details/gsgylyqhr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gkpqfnxvc.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/gnyjbzcjs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gzoggpnei.sHtML

[R34] 退出时清理
来源：http://baike.zdbjq.cn/Article/details/gkuzdvprj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gpxxckzza.sHtML

[R35] 后台执行并等待
来源：http://www.share.zdbjq.cn/Article/details/gzdbailyc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/gmbjizdry.sHtML

[R36] 并发执行多个任务
来源：http://mobile.hesvh.cn/Article/details/gmjpstcfg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/gobawctpu.sHtML

[R37] 把输出赋给变量
来源：http://blog.zdbjq.cn/Article/details/gekmwzhjn.sHtML

files=$(ls -1)
来源：http://3g.hesvh.cn/Article/details/gwrrrjnbk.sHtML

[R38] 管道串联
来源：http://blog.fehbvm.com/Article/details/gosiahxtp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.zdbjq.cn/Article/details/gbxmxiaat.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fehbvm.com/Article/details/gimjjbcxq.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gaytnucga.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/guykjmsih.sHtML

echo "log" >> out.log
来源：http://read.share.hesvh.cn/Article/details/ghykcpfvc.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/gmutsfagd.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fehbvm.com/Article/details/gvqkyhbst.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/grxnynkrc.sHtML

wc -l < a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gfvsudukt.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/gyxbtfwqg.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/ghnfoavab.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/gmklosdrt.sHtML

find . -mtime -7 -type f
来源：http://wap.zdbjq.cn/Article/details/gpmqixqvt.sHtML

[R45] 批量删除
来源：http://baike.hesvh.cn/Article/details/gbulvsvxp.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.zdbjq.cn/Article/details/gqtihinne.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/gsgxyzakl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.zdbjq.cn/Article/details/gtylijdro.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/gfpffivrt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gfzvkliir.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/gpuupnzus.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.hesvh.cn/Article/details/gujbyjggk.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/gstfjwrxd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fehbvm.com/Article/details/gmuqncsxk.sHtML

[R50] awk 求和
来源：http://www.m.share.zdbjq.cn/Article/details/gisoudcbf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/guxorvpca.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/gycqfkssb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fehbvm.com/Article/details/gbrjscihr.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/gjglikflu.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/ghjciudps.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.zdbjq.cn/Article/details/glngmqiml.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.zdbjq.cn/Article/details/gnvfgfedy.sHtML

[R54] 比较两个文件
来源：http://www.m.share.hesvh.cn/Article/details/gkmzeaddw.sHtML

diff a.txt b.txt
来源：http://m.share.fehbvm.com/Article/details/gtvjqzbxj.sHtML

[R55] 压缩与解压
来源：http://m.share.zdbjq.cn/Article/details/ggnvjtmoo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gtcaxzytb.sHtML

[R56] 远程拷贝
来源：http://www.blog.fehbvm.com/Article/details/gpqghrejs.sHtML

scp file user@host:/path/
来源：http://blog.fehbvm.com/Article/details/gntblzftj.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/gclnldhhw.sHtML

ssh user@host 'uptime'
来源：http://m.share.zdbjq.cn/Article/details/gsexuzden.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/gmtktnoqi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fehbvm.com/Article/details/gzddjvrca.sHtML

[R59] 发 POST JSON
来源：http://wap.hesvh.cn/Article/details/gujkoomoy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.hesvh.cn/Article/details/gxvoiliye.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gciqngjml.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.hesvh.cn/Article/details/guhzgfyhx.sHtML

[R61] 磁盘占用
来源：http://3g.zdbjq.cn/Article/details/gzkhqactf.sHtML

df -h;  du -sh *
来源：http://m.share.fehbvm.com/Article/details/grrncurhy.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/gkmprcbal.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.zdbjq.cn/Article/details/gtmiznbhu.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gxwhiopfc.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/gijrsthvr.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/ggrutajva.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/guohugdqz.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/gmxacqhwf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.hesvh.cn/Article/details/gnjgcwled.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/gdrchekir.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gwplljdsc.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/gdyooxvpj.sHtML

openssl rand -hex 16
来源：http://www.m.share.hesvh.cn/Article/details/gkfbeqwia.sHtML

[R68] 计算文件校验值
来源：http://www.blog.zdbjq.cn/Article/details/ghsgzpcnf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fehbvm.com/Article/details/gsrdqdjda.sHtML

[R69] 生成随机密码
来源：http://m.share.hesvh.cn/Article/details/gmgmetjkh.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gjualvvbl.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/ggoovdwrl.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.zdbjq.cn/Article/details/guyhbainq.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/guizojnif.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/gfjtanlsd.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/gbizhjwfu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gkrqzgphl.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/gkvqccvmi.sHtML

split -l 1000 big.log part_
来源：http://mobile.hesvh.cn/Article/details/gbrzrfhwr.sHtML

[R74] 批量重命名
来源：http://www.share.hesvh.cn/Article/details/grneanegv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.hesvh.cn/Article/details/gychybvfu.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gwghectmw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.hesvh.cn/Article/details/gbjdwzvak.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gadzlmxvx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gvnfjcqwb.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/gtkumzcci.sHtML

read -rp "请输入: " ans
来源：http://wap.hesvh.cn/Article/details/gauplsgzl.sHtML

[R78] 交互式菜单
来源：http://www.m.share.hesvh.cn/Article/details/gaqlbibor.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/ghawfgkdv.sHtML

[R79] 解析命令行选项
来源：http://3g.zdbjq.cn/Article/details/gfqwupoqt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/glroanquv.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.zdbjq.cn/Article/details/gauvsedna.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/gzxatpzrd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ginoejiyd.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/gmwpwvutq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gphhcaxrv.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/gvhvsqykq.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/gswyabccd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/gfrxqceqg.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.zdbjq.cn/Article/details/goihluvek.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.zdbjq.cn/Article/details/gdsncjrco.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/grkqiocmh.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/gkcayutgc.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/gwmsevdxc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/grkleasdw.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gwfulylwx.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gjtuwbhev.sHtML

[S06] C：字符串比较
来源：http://www.share.fehbvm.com/Article/details/gsfnrdorj.sHtML

strcmp(a, b) == 0
来源：http://m.share.hesvh.cn/Article/details/gewepbflk.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/glnolmuou.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/ghxelpbyp.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/gvqmqxqfe.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/gwufsqlgd.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gbehykjit.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/ggwmfxuph.sHtML

[S10] C：指针与解引用
来源：http://m.share.zdbjq.cn/Article/details/gszluusvk.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/gwtpmoqbc.sHtML

[S11] C：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gnyxeqgzs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/gtijvgdfj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.zdbjq.cn/Article/details/gewqijvxt.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gxqxbwggb.sHtML

[S12] C：写文件
来源：http://mobile.fehbvm.com/Article/details/gptimdleq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gcgpezhdw.sHtML

[S13] C：宏定义
来源：http://read.share.zdbjq.cn/Article/details/grezczkoq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fehbvm.com/Article/details/gbreayjza.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/grxmiadsf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.hesvh.cn/Article/details/gcxjvoaqm.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gfmceuwda.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/gtrvpmsnw.sHtML

[S16] C：位操作置位
来源：http://blog.hesvh.cn/Article/details/glradwmab.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/ganrmcsbw.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gphipbcsy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/gxxadpwll.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/gbfuguvbg.sHtML

int main(int argc, char **argv)
来源：http://blog.hesvh.cn/Article/details/gccawmmqa.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/ggzprvywd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/grwcsllad.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gfzdysavf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gtnayojcb.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/gkfnjzgeo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fehbvm.com/Article/details/gkaawhvkz.sHtML

[S22] C：字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gauiuqyvk.sHtML


<!-- 参考信息 -->