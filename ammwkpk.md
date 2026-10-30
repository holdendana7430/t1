代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gaaknbzun.sHtML

[Q50] 批量更新
来源：http://wap.fanxiaobao.xyz/Article/details/giubhtczk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsztejydz.sHtML

[Q51] 用子查询更新
来源：http://3g.fanxiaobao.xyz/Article/details/gqjbfjaol.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/grhudoszt.sHtML

[Q52] 删除指定行
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqgfgnts.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/giarhxxfw.sHtML

[Q53] 按条件删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpvffatz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnzkorry.sHtML

[Q54] 清空表
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvqjirtw.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fanxiaobao.xyz/Article/details/gypawbxid.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhnojdge.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjsyqrzn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gyycgojbp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkydeeqtv.sHtML

[Q57] 行号
来源：http://baike.fanxiaobao.xyz/Article/details/gbrrsecog.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gchuupsaq.sHtML

[Q58] 累计求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzyfigbx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjwkykew.sHtML

[Q59] 分组内累计
来源：http://wap.fanxiaobao.xyz/Article/details/gsxcvtjzu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaemgtrvx.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqbsqcyz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrirbtzs.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnsajnbdl.sHtML

[Q61] 移动平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbwuirgt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqzugbhc.sHtML

[Q62] 分组占比
来源：http://m.share.fanxiaobao.xyz/Article/details/gyefzibxy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjtejxak.sHtML

[Q63] 开启事务
来源：http://3g.fanxiaobao.xyz/Article/details/gdjzdxxzo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fanxiaobao.xyz/Article/details/gibtetwsd.sHtML

[Q64] 提交事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbeiqttbt.sHtML

COMMIT;
来源：http://baike.fanxiaobao.xyz/Article/details/gxbdckjxm.sHtML

[Q65] 回滚事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpgxbkwl.sHtML

ROLLBACK;
来源：http://baike.fanxiaobao.xyz/Article/details/gkpgtnatv.sHtML

[Q66] 行锁查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gicqmvthe.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fanxiaobao.xyz/Article/details/glwqyyloj.sHtML

[Q67] 设置隔离级别
来源：http://wap.fanxiaobao.xyz/Article/details/gkliszeai.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fanxiaobao.xyz/Article/details/gsahnzbmu.sHtML

[Q68] 保存点
来源：http://wap.fanxiaobao.xyz/Article/details/gjgnugxfq.sHtML

SAVEPOINT sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjjohkok.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbuvqzbj.sHtML

[Q69] 查看执行计划
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvsdixvg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxnghohm.sHtML

[Q70] 更新统计信息
来源：http://wap.fanxiaobao.xyz/Article/details/gkbbhqlde.sHtML

ANALYZE TABLE users;
来源：http://3g.fanxiaobao.xyz/Article/details/gvgawxxkd.sHtML

[Q71] 查看建表语句
来源：http://3g.fanxiaobao.xyz/Article/details/gsprpawlp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fanxiaobao.xyz/Article/details/genxfhzgg.sHtML

[Q72] 查看索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbetubkk.sHtML

SHOW INDEX FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gvemcqtvu.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/giakiyyzr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqniafsus.sHtML

[Q74] 强制使用索引
来源：http://www.share.fanxiaobao.xyz/Article/details/grluwovlq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpoamanet.sHtML

[Q75] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gezaqcodc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwswfkoe.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fanxiaobao.xyz/Article/details/gqeaqimky.sHtML

[Q76] 按天统计
来源：http://m.share.fanxiaobao.xyz/Article/details/glcdmnwpi.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fanxiaobao.xyz/Article/details/gilddvfkw.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/gayyzjrkc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydoiqzoi.sHtML

[Q78] 当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcziyxyg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fanxiaobao.xyz/Article/details/gpkmldnah.sHtML

[Q79] 字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gggdnjojc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guimzsubk.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtkqwqen.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gocqsebfu.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gegkuizbc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gftbgbicj.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/grptftwyq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/goaetphgc.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gxuynfywm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrerclzh.sHtML

[Q84] 去除首尾空格
来源：http://blog.fanxiaobao.xyz/Article/details/gtcrzjtyj.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gfsgnzmnt.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/gawlxynan.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/goagrarro.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/gxgdchtbh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glclabuxj.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gyyiibwar.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/gejcnhggd.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gcrqwmxnz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmebhssp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gplqtuisg.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gwiuspvbg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcjqpxuu.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnidnqtml.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fanxiaobao.xyz/Article/details/gtnehieek.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gqorirzmx.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgmivoar.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfppykym.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdmkoutz.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/gsnmfbisg.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/goehbjlxy.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfddkmksf.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvuwcujlf.sHtML

[R03] 只读变量
来源：http://blog.fanxiaobao.xyz/Article/details/gnumqebjm.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/grrxqkdwo.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/gdckmszdp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvutjgus.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljxqtmtd.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnncduzzu.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gnbgnpyos.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtixitqes.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/guyfnfzns.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfazjhfq.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhizjoko.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gdnvrodhb.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gzqkuwcle.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gontytehm.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyvvpfsr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gfgyvpzvd.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhcfeqap.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gvlhnlbap.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsysuedv.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmakrqbh.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwwblqnw.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gosuxddvu.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gtyndsqet.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gzfvsudct.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gorlmytha.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gyfbhnpfm.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqdefcnx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkkseqmc.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlavpfbt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gtjpttvyx.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwxojbby.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmvzjiza.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjpxxcfn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gcuerxamu.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gcoxwzcbn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gtjdmoflj.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gldaqgxel.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqjwqidf.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggniijksg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsleucdo.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlhdxpgo.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gobspiozb.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gysiznzgf.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gngftejtg.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gzqsterme.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gguourgin.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gycmamots.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gczmhdfgd.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/goglccgmx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/ghxmeehfr.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhqtdiyb.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/gfsmyunph.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gftvscczq.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnkvlahp.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/grbmeewsi.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjkcjmax.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gmesvnwdp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyqgdbjp.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxqcnjwp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gjngprkrc.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpfivuty.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/ggbgsuato.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gnfxjcggf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevzyugfm.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/ggjunneag.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqdmcnjg.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/geepkdxvp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/guyjxgsef.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gwndqwsmy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gtuduvwxy.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gfifepcuf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/gnzhozqtk.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gyvzkkrzy.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gegmtapux.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/giibcbesh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfutoeyz.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsazfkykh.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gaecflqtt.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/guzkbjkxg.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/grhgmjbxr.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gatydxqew.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gswpjiruy.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/gutmssykj.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/grhpdojtg.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gmtguoiyk.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gzxhmlqin.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhbejkwi.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gtpzhznap.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gmiuxweek.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggchdynoa.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbtthmku.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/glijgnztd.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdepasxh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzipvckx.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/ghiqmadup.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gkmcmklhz.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gwdvmgysa.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gsezqgpan.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gwptfnayb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzzhiyfn.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmecbmeg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgstynud.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybasufjk.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/ghwnldhdj.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grefuiaum.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwwsgchq.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gbuwmdvpf.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchlddfst.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/giknxflfl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gykyfuyjh.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gtdtdncsv.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/grlfgjdes.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjxwlzne.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gyynqfxmc.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/geklkydha.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/ghwhbzpjz.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gstqvjsnt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgwjsoeo.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gluymsiop.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekleqhbt.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpnuefsq.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnvysris.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gekaujujf.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gzweupmka.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gzwdftgtz.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbgqjzev.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfvtffqe.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gapopfxrd.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgmmtxkw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gdeahrvzq.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhbaojaa.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/glmatkcub.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gnveawdcu.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/gxbynsvlk.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfaohzhv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnknlkdc.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsrflgcg.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzkflzua.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gwjxutvrn.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gysbmpzur.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqfcbjly.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gyuzaqzwp.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gyfnvshgu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/guvumbkkt.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnqappvs.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpyvbrcj.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gizsbtgev.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gknhkqxnt.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gshughtfi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/guzmgvrco.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/glebfydog.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/geiievgdo.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gptnjuafi.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gcnbdenqc.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/geobzqmuq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gizlpizja.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/grstsckps.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gvomunnri.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/gemrkhpwo.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/gpuokzzvj.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfrlgkjx.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfdnrvfg.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gsspoztml.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwtzryke.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixmltssr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqtkwgpf.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/geenxeugt.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gokrxfrzi.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkufiixll.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxeogmvlj.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggraldope.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gbwkgahto.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlbxxzaj.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbamtpyo.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsubvdiz.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/gpdvxkrfe.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkafgovs.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gusaqufkn.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gmnoptgtm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmsexntk.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gbmjowxjz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkcnriwb.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdiynxet.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gijiwkjai.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gbnsffvke.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhcviwrs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gajvbmnpg.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gzqyjygad.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gehdehaos.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gtlmlkzsq.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gvrrshcbr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggnlutsu.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkhkgcyr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gtspcnbhc.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkcglzlz.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfpcbodk.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvresdeit.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gnnzquvkc.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gwrvlszrt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggeslzthv.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gwkvldtju.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/guoyhmjhw.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gudcxogbi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gqepgkirz.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwhipkpa.sHtML


<!-- 参考信息 -->