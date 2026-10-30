代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/gvzrtxsjz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/ggthnmznp.sHtML

[Q47] 与平均值比较
来源：http://baike.fehbvm.com/Article/details/gnqbuohbn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fehbvm.com/Article/details/gydmbwtmd.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.hesvh.cn/Article/details/gnbpebthq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/gtalraiya.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fehbvm.com/Article/details/gsjgkxdgg.sHtML

[Q49] 更新单行
来源：http://www.share.zdbjq.cn/Article/details/ganpspswl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/giwtuxbxl.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/gtoqndpab.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fehbvm.com/Article/details/gkxrnwhwv.sHtML

[Q51] 用子查询更新
来源：http://3g.fehbvm.com/Article/details/gwintfucp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fehbvm.com/Article/details/gynfzquvi.sHtML

[Q52] 删除指定行
来源：http://baike.hesvh.cn/Article/details/gdsmrlolo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gfxahqqvp.sHtML

[Q53] 按条件删除
来源：http://read.share.fehbvm.com/Article/details/gdlrbzsvn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gmyswtdjo.sHtML

[Q54] 清空表
来源：http://blog.hesvh.cn/Article/details/gkeqehdqa.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fehbvm.com/Article/details/gopvxaycu.sHtML

[Q55] 排名（并列占位）
来源：http://wap.zdbjq.cn/Article/details/gfpjppnco.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/gwxhnvtlg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.zdbjq.cn/Article/details/gtrygibld.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.hesvh.cn/Article/details/glbwudzbd.sHtML

[Q57] 行号
来源：http://mobile.fehbvm.com/Article/details/gihrarxpb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/gemtghgyk.sHtML

[Q58] 累计求和
来源：http://baike.zdbjq.cn/Article/details/gtltnpvpq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.hesvh.cn/Article/details/guaiquvwe.sHtML

[Q59] 分组内累计
来源：http://blog.fehbvm.com/Article/details/gafiqkljq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gctfzychx.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.hesvh.cn/Article/details/gyhgsfbhs.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fehbvm.com/Article/details/guqkofukg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fehbvm.com/Article/details/gwdncwrib.sHtML

[Q61] 移动平均
来源：http://m.share.zdbjq.cn/Article/details/gfuikerjf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gkmyrqjjh.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/gqgecmzqv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gbjnwsbxb.sHtML

[Q63] 开启事务
来源：http://baike.hesvh.cn/Article/details/ggarhnmjx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.hesvh.cn/Article/details/gbtzaltlt.sHtML

[Q64] 提交事务
来源：http://www.blog.hesvh.cn/Article/details/gmscuzofz.sHtML

COMMIT;
来源：http://www.m.share.hesvh.cn/Article/details/gizcytekc.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/gbuiumpnd.sHtML

ROLLBACK;
来源：http://www.blog.zdbjq.cn/Article/details/godrlckaf.sHtML

[Q66] 行锁查询
来源：http://www.share.hesvh.cn/Article/details/glysrsoms.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fehbvm.com/Article/details/gqviumwmu.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fehbvm.com/Article/details/grytskjdv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.zdbjq.cn/Article/details/gxjcdbfxa.sHtML

[Q68] 保存点
来源：http://www.blog.hesvh.cn/Article/details/gogwsfdqr.sHtML

SAVEPOINT sp1;
来源：http://baike.fehbvm.com/Article/details/giyykqjer.sHtML

ROLLBACK TO sp1;
来源：http://www.share.zdbjq.cn/Article/details/gctnrlyzz.sHtML

[Q69] 查看执行计划
来源：http://blog.zdbjq.cn/Article/details/gsfybfeob.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.zdbjq.cn/Article/details/geibygdyr.sHtML

[Q70] 更新统计信息
来源：http://wap.zdbjq.cn/Article/details/gnfbxpksy.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.hesvh.cn/Article/details/gtoefyamt.sHtML

[Q71] 查看建表语句
来源：http://www.share.fehbvm.com/Article/details/ghqkxfblx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.zdbjq.cn/Article/details/gzgwtshbc.sHtML

[Q72] 查看索引
来源：http://wap.hesvh.cn/Article/details/gvxgmoekz.sHtML

SHOW INDEX FROM users;
来源：http://3g.hesvh.cn/Article/details/gbnjwdqpx.sHtML

[Q73] 查看表状态
来源：http://read.share.fehbvm.com/Article/details/gbqekrbxa.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.hesvh.cn/Article/details/geuyonvhv.sHtML

[Q74] 强制使用索引
来源：http://mobile.fehbvm.com/Article/details/gozueaioy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.zdbjq.cn/Article/details/gzwypajww.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gfmlswuxc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.hesvh.cn/Article/details/gebpkhtps.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/gifaygefe.sHtML

[Q76] 按天统计
来源：http://read.share.zdbjq.cn/Article/details/gyiztvhah.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.zdbjq.cn/Article/details/gfcjmzrdo.sHtML

[Q77] 时间加减
来源：http://m.share.hesvh.cn/Article/details/gxopwjaub.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.hesvh.cn/Article/details/glwpkgoat.sHtML

[Q78] 当前时间
来源：http://m.share.hesvh.cn/Article/details/gqnrtmmce.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.hesvh.cn/Article/details/gfsnphudj.sHtML

[Q79] 字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gevhbtibu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fehbvm.com/Article/details/gougwyosi.sHtML

[Q80] 字符串截取
来源：http://read.share.zdbjq.cn/Article/details/gngtadolk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gbdkivmsf.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gyigzptex.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gxxcdjdrc.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fehbvm.com/Article/details/gihqnynfg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/glzszibgv.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/getbzifaw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gzuarbknj.sHtML

[Q84] 去除首尾空格
来源：http://3g.zdbjq.cn/Article/details/gzaoczsvc.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gynlienxl.sHtML

[Q85] 数值取整
来源：http://mobile.zdbjq.cn/Article/details/gwkjqltbz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.hesvh.cn/Article/details/gzudragqm.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/gtuuzdlns.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fehbvm.com/Article/details/gcmkgkcsp.sHtML

[Q87] JSON 字段做条件
来源：http://baike.hesvh.cn/Article/details/gffwvklfx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/gnkqpzeto.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/gkejyivsl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.zdbjq.cn/Article/details/gmyjkmidl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gdecvgpcv.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gosyescsj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.hesvh.cn/Article/details/gzehslone.sHtML

[Q90] 生成序号列
来源：http://www.m.share.hesvh.cn/Article/details/gwmcxswzb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fehbvm.com/Article/details/gpfjnbvqn.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqwjnjgeo.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/gecllvtbk.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/geaauikgl.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/gpemmftgf.sHtML

#!/usr/bin/env bash
来源：http://3g.zdbjq.cn/Article/details/gygbmzzxh.sHtML

set -euo pipefail
来源：http://read.share.fehbvm.com/Article/details/gvapeeqyq.sHtML

[R02] 变量赋值与使用
来源：http://m.share.zdbjq.cn/Article/details/gcaaoekke.sHtML

name="Tom"; echo "$name"
来源：http://read.share.hesvh.cn/Article/details/ghtbattpq.sHtML

[R03] 只读变量
来源：http://m.share.fehbvm.com/Article/details/gelaivklr.sHtML

readonly PI=3.14
来源：http://mobile.zdbjq.cn/Article/details/gmbxgcdfp.sHtML

[R04] 位置参数
来源：http://read.share.zdbjq.cn/Article/details/gzwazbynl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/ggxtmhnsv.sHtML

[R05] 参数默认值
来源：http://mobile.hesvh.cn/Article/details/gcmqzuodp.sHtML

name="${1:-default}"
来源：http://3g.fehbvm.com/Article/details/gacpdrbdx.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fehbvm.com/Article/details/gwkelqsjd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gfcxqympl.sHtML

[R07] if 判断文件
来源：http://3g.fehbvm.com/Article/details/gmkbxzgxb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.hesvh.cn/Article/details/gbkhyqfsw.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/gvevnnfep.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.hesvh.cn/Article/details/gwqxbssge.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gdipgrogv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gwiaxvdgg.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/guhbnbuaa.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fehbvm.com/Article/details/gypqmsxlb.sHtML

[R11] case 多分支
来源：http://www.share.zdbjq.cn/Article/details/gpmijqprs.sHtML

case "$1" in
来源：http://3g.zdbjq.cn/Article/details/gkhyrydmu.sHtML

start) echo "启动" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gqqfauljc.sHtML

stop)  echo "停止" ;;
来源：http://blog.fehbvm.com/Article/details/gfgnobwmn.sHtML

*)     echo "未知命令" ;;
来源：http://wap.hesvh.cn/Article/details/ghoeijcfg.sHtML

esac
来源：http://wap.fehbvm.com/Article/details/gqvopgitt.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/gsearayql.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/ghefzzhel.sHtML

[R13] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/gengcnswy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/ggeyeuxat.sHtML

[R14] C 风格 for
来源：http://mobile.zdbjq.cn/Article/details/gdgscbjvc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/grswqlduo.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/gvzavrwrs.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.hesvh.cn/Article/details/ghkshzicx.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/gdcihvulf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gbyuwjjas.sHtML

[R17] 数组定义与取值
来源：http://m.share.zdbjq.cn/Article/details/gzbapzakw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.hesvh.cn/Article/details/gruqrqukx.sHtML

[R18] 遍历数组
来源：http://m.share.hesvh.cn/Article/details/gjwuuusze.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/glfewhpls.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gbkbgvyac.sHtML

echo "${#arr[@]}"
来源：http://m.share.hesvh.cn/Article/details/gjkwicave.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fehbvm.com/Article/details/gasfdbyhd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.zdbjq.cn/Article/details/gftrvjpro.sHtML

[R21] 字符串长度
来源：http://mobile.fehbvm.com/Article/details/gdmygqkln.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/gmolxrete.sHtML

[R22] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gvryxdnzm.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/gvgzeluvc.sHtML

[R23] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/ghoijbser.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/gwueztugv.sHtML

[R24] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/ggcgqnvms.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.hesvh.cn/Article/details/gktptidyh.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.hesvh.cn/Article/details/goosivehe.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/gklegswgh.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/glmpgomwe.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.hesvh.cn/Article/details/gmkohuusk.sHtML

[R27] 算术展开
来源：http://mobile.fehbvm.com/Article/details/gsnidxjoi.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fehbvm.com/Article/details/ghpetteta.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/gjiuemdao.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/gbphmkvqz.sHtML

[R29] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gskofwuzw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.hesvh.cn/Article/details/gvxfjgkrt.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/gxevbtsns.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fehbvm.com/Article/details/gtzvvepvr.sHtML

[R31] 局部变量
来源：http://read.share.zdbjq.cn/Article/details/gksoikayu.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.hesvh.cn/Article/details/gydxebpcu.sHtML

[R32] 参数个数校验
来源：http://mobile.fehbvm.com/Article/details/gmlypqiuc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gqopdovft.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.zdbjq.cn/Article/details/gchhzlcrh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.zdbjq.cn/Article/details/gbdembgnq.sHtML

[R34] 退出时清理
来源：http://mobile.fehbvm.com/Article/details/gslcavpmn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/goxywyatc.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/gusdjagaa.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/gsapmmows.sHtML

[R36] 并发执行多个任务
来源：http://blog.hesvh.cn/Article/details/gnrfvvdlq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.hesvh.cn/Article/details/ghmptdyah.sHtML

[R37] 把输出赋给变量
来源：http://blog.hesvh.cn/Article/details/gxqvcjfhd.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/gtncwksjc.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/govoyedxk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/gdkpmupoq.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fehbvm.com/Article/details/gjuwljtly.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/gkunalkvd.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/gtojmhupo.sHtML

echo "log" >> out.log
来源：http://baike.fehbvm.com/Article/details/gpkjtujno.sHtML

[R41] 丢弃输出
来源：http://www.share.zdbjq.cn/Article/details/gbfesxloy.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gjqtefted.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/gbjphtofu.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/glfsvybvw.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/gwilgnljw.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.hesvh.cn/Article/details/gfwlchajv.sHtML

[R44] 按修改时间查找
来源：http://m.share.zdbjq.cn/Article/details/gvgbidtak.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/gnaevakyc.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/gorvulynl.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/gddwqlast.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.hesvh.cn/Article/details/gfydfeehc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fehbvm.com/Article/details/geofkydha.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fehbvm.com/Article/details/gkxuweawl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/gbrdduicb.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gjktyxlul.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/ggdjdawzg.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/gozsyxuhk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/gexyhubbb.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/gwjwdvqyj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gkgctyywz.sHtML

[R51] 排序去重取前几
来源：http://blog.zdbjq.cn/Article/details/gxihfrlon.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gkcawxzsj.sHtML

[R52] 统计行数
来源：http://wap.zdbjq.cn/Article/details/gnqqqtbvs.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/gpvrcmure.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/gsxyqrbop.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/gcgclaizh.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/gzohzlsho.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/grfjaislx.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/gqnqoweoy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fehbvm.com/Article/details/gzzeelrph.sHtML

[R56] 远程拷贝
来源：http://wap.fehbvm.com/Article/details/guyrnsjwn.sHtML

scp file user@host:/path/
来源：http://read.share.zdbjq.cn/Article/details/gzrjptvzl.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/gfcvfvamj.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.hesvh.cn/Article/details/gcorzpjnu.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/gbgfouqje.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/gwbyhmryi.sHtML

[R59] 发 POST JSON
来源：http://baike.hesvh.cn/Article/details/gmruzuzqs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.zdbjq.cn/Article/details/gmhbtohvk.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gjwheoubb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/gmnuhlspz.sHtML

[R61] 磁盘占用
来源：http://mobile.fehbvm.com/Article/details/gktbarbot.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/ggvddygzj.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/ggsywdzvp.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/gpbvcwofj.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gpkilmmqo.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.zdbjq.cn/Article/details/guunbbtik.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/gctgjitle.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/gbdjffepl.sHtML

[R65] 查看端口占用
来源：http://baike.zdbjq.cn/Article/details/gcprnikka.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.zdbjq.cn/Article/details/guzuyypvi.sHtML

[R66] 定时任务
来源：http://mobile.zdbjq.cn/Article/details/gkgakgjvf.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/gwbhywqua.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/gqxfjqrmc.sHtML

openssl rand -hex 16
来源：http://mobile.hesvh.cn/Article/details/gjpwwgnhb.sHtML

[R68] 计算文件校验值
来源：http://mobile.hesvh.cn/Article/details/gtwvzglqu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fehbvm.com/Article/details/gswqyytqn.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/gzcjqyvmq.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gddorkyll.sHtML

[R70] 时间戳与互转
来源：http://blog.zdbjq.cn/Article/details/gpgqlcmvh.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/gethotzmp.sHtML

[R71] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gjnudwrhc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fehbvm.com/Article/details/grblgtkyx.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gpkvvfdec.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gqrlkhgkc.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/grzutndpn.sHtML

split -l 1000 big.log part_
来源：http://www.share.zdbjq.cn/Article/details/gzeddxwre.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/gvgwajcem.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.zdbjq.cn/Article/details/ghygpbigj.sHtML

[R75] 导出环境变量
来源：http://wap.fehbvm.com/Article/details/gtyenumrw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/gdscjntfx.sHtML

[R76] 使用临时文件
来源：http://wap.fehbvm.com/Article/details/gyosxkkdv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gisdmdhvz.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/gtpposlvo.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gedycclva.sHtML

[R78] 交互式菜单
来源：http://m.share.hesvh.cn/Article/details/gqjixiozv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/gawhecmsn.sHtML

[R79] 解析命令行选项
来源：http://www.share.zdbjq.cn/Article/details/gzmitwrao.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/gpewyjuqa.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fehbvm.com/Article/details/gytthdtap.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/gdbrrqtbh.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gyztlvtbi.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/gnljxjzpl.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/guayqdgrm.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/gqyqwzvsj.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/gaqavcpae.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/gxyrjtvaw.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fehbvm.com/Article/details/gelmrutfm.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.zdbjq.cn/Article/details/ginyiqjzh.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gepqnwayd.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/gkfuvuisb.sHtML

[S04] C：字符串复制
来源：http://read.share.zdbjq.cn/Article/details/gsvnoeatw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/gbwusmtvs.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gdjtiympu.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/gejtstitz.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gdorvcrdc.sHtML

strcmp(a, b) == 0
来源：http://www.share.zdbjq.cn/Article/details/gegrtmfip.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/gczquscwy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/gyymhnqcj.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/gxcwmcvnn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.zdbjq.cn/Article/details/glscofifw.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.zdbjq.cn/Article/details/gcflnpcma.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gbzvdcpqp.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/grvksqxjy.sHtML

int *p = &a;  *p = 5;
来源：http://wap.zdbjq.cn/Article/details/gweudiuzm.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gspsvwgga.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/genyzveze.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/gmulgqlpg.sHtML

fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gtwppgheu.sHtML

[S12] C：写文件
来源：http://www.blog.fehbvm.com/Article/details/gtqzcksmq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gzdgoihgi.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/gixjwjjkf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/gwbjqunvf.sHtML

[S14] C：枚举
来源：http://mobile.zdbjq.cn/Article/details/gcwfakbfh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/gmqiyzkoe.sHtML

[S15] C：类型转换
来源：http://m.share.fehbvm.com/Article/details/gyhomzvxo.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/gzgovsgpp.sHtML

[S16] C：位操作置位
来源：http://wap.hesvh.cn/Article/details/gsaojenhq.sHtML


<!-- 参考信息 -->