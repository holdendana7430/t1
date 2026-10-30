代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwlpkokt.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavrnnwid.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gzwawablu.sHtML

[Q53] 按条件删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gpyyahwgf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gnnastskw.sHtML

[Q54] 清空表
来源：http://m.share.fanxiaobao.xyz/Article/details/giihwiwcr.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggprzvosv.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fanxiaobao.xyz/Article/details/gpzytxouv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpulcccgu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxznyoiy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gyhbmzdit.sHtML

[Q57] 行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtpequxf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gqkztcnhx.sHtML

[Q58] 累计求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqplgdnj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/ghxkfkapf.sHtML

[Q59] 分组内累计
来源：http://wap.fanxiaobao.xyz/Article/details/gpliivhyb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxutnqmc.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrxatyrn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxgvimli.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gduotvrus.sHtML

[Q61] 移动平均
来源：http://baike.fanxiaobao.xyz/Article/details/gitrzuyug.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/goncjseet.sHtML

[Q62] 分组占比
来源：http://read.share.fanxiaobao.xyz/Article/details/gmoptahph.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gjjrwwokd.sHtML

[Q63] 开启事务
来源：http://wap.fanxiaobao.xyz/Article/details/gnltchvdr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikppljxl.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkzyltoy.sHtML

COMMIT;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfsrpxsp.sHtML

[Q65] 回滚事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnspruzp.sHtML

ROLLBACK;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtailiey.sHtML

[Q66] 行锁查询
来源：http://3g.fanxiaobao.xyz/Article/details/gqtewemyy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fanxiaobao.xyz/Article/details/gifftonlx.sHtML

[Q67] 设置隔离级别
来源：http://baike.fanxiaobao.xyz/Article/details/gmnkrpqbb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fanxiaobao.xyz/Article/details/ggglatolc.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/gakqdwhlw.sHtML

SAVEPOINT sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/ghdkdwbyh.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/grhbykmtf.sHtML

[Q69] 查看执行计划
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyyayenj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fanxiaobao.xyz/Article/details/gixagaobm.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtecqirt.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjaobxsh.sHtML

[Q71] 查看建表语句
来源：http://blog.fanxiaobao.xyz/Article/details/gxyabpsfl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygfanqke.sHtML

[Q72] 查看索引
来源：http://read.share.fanxiaobao.xyz/Article/details/garsaofth.sHtML

SHOW INDEX FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gsumwzfac.sHtML

[Q73] 查看表状态
来源：http://baike.fanxiaobao.xyz/Article/details/gnpyociyg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/glcrmqerm.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/ggsguzxrz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fanxiaobao.xyz/Article/details/giuomtjoe.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpfbsrjl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gbzkphjkn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjijxgxeh.sHtML

[Q76] 按天统计
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjeplkkb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fanxiaobao.xyz/Article/details/gpfstbeyh.sHtML

[Q77] 时间加减
来源：http://mobile.fanxiaobao.xyz/Article/details/gygmwnjbq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fanxiaobao.xyz/Article/details/glmztroyk.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzkwpodh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfcboklw.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavgzmwxr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdzstrfh.sHtML

[Q80] 字符串截取
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlyloddf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gqwvdvtyi.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvjyweos.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbmbubty.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvcrucvv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gfkxkfvpw.sHtML

[Q83] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvmcjsfl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvprmtws.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflyfqgxd.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxmagdto.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpbeoauq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjegrgqbt.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fanxiaobao.xyz/Article/details/gmypihflo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/gvxmgsphp.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/geirmajcv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/gjrshooui.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fanxiaobao.xyz/Article/details/gjosftnqb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnnrcjcq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gehbjacqp.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwwefqwn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkoasexx.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsoantvm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gpqnhrilz.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gegxznqet.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpysgjhyr.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gcunfjuax.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqllrubrk.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/gcufjmecj.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdmkuymp.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/gkzslryyl.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyayanxtd.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gkicnqqys.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjlorfto.sHtML

[R04] 位置参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwpibead.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtyaknnte.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtgluwkt.sHtML

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmixzqfr.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfoetwvvy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gteyeyefv.sHtML

[R07] if 判断文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxlorxlj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpyhjpqqk.sHtML

[R08] 数值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgjanoih.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncrtvshh.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/ggryupfei.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/ggquwuqlj.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gbhnnrtbu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gbdvdpmtp.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/gxheayezj.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdzhyupc.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/grtqoafnz.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/godvbifou.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtauyhzlv.sHtML

esac
来源：http://3g.fanxiaobao.xyz/Article/details/gyjvvqhun.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymimlpix.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gamjpodhs.sHtML

[R13] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/gyqikfaxl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gvwslobfv.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggytafeto.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/grzyrwpdj.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gokcgwyor.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gerytedrt.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gfthhbqnw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcqligbk.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/gddwpbjzs.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrlhtpfw.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gljbwiuey.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfmwbrmr.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpsutupa.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwfbkubt.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzadrchr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gdwfybjix.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gczwnyyvp.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gguktphkz.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhvqkbrh.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/gjwhobbrj.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gytrskgmd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/ggxedthft.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gmnbzwgiq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gehhvhcfu.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gnipddlxd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gukwqtrpo.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gezztrbdp.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/gbacmakok.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomqyigrt.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgdpapzv.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gwscbqsxy.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gpabgytoz.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gdjjyyzbk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/ggslknwbi.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gostcfkbh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpbqbeza.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giiehjwtl.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfqqdgne.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gxqervugy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbbjhczvx.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gpeqpxsmx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gxausyzcs.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdlrxjzw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqzwonme.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/ggfnmiokw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gfjksvrhn.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/giumvlgsw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxvouzfx.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/giegzwmtr.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhvxxdgn.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gowbnhttc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvxafjba.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrdivaex.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskdyudil.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gmlxqtgkj.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/glbdilzrw.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gykomasua.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gafpxcvzu.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gyacrkmxo.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gtyrzmwmp.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gtksukexl.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdpathlk.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gnpzdbggp.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpijgnzq.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gytcilutl.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gbsrjkqka.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/goqvngdnj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gkzebtzmf.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/gvlyopcgm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gdajbiwbp.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnkimwqo.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnurwexdb.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbchbitr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzcfrihg.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/gkpwprxxo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdvyqfun.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gabkjsqeo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gkudfcgjk.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gujubbkup.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gleslgcoy.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/grgztflxd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvwzlxol.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcgdybxj.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gpludqrss.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvvnhkko.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gtvnlrolb.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/goxijitye.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gigeyjgmc.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbayifcfg.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gpljdkprg.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkuynsck.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/glbdtfdki.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfcjslvp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/grtkmlheh.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdmjviey.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/ghyyldrsn.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbptgsbrt.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gfjemypsq.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbsnbfxhg.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhdeikmm.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbdzrmte.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqympfdlw.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtbwnonx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glghpgqzt.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gvwqntbzl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gnixftrtt.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gtdgffrjz.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gcefzdefr.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gtvgamujd.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaztrepnj.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/gsifidwls.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gruvwqedu.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvjvsriw.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gabbtlqdx.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gblfbswgs.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gtowaknuj.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gwghmuqvj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxibdzpm.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftqvzwkq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gijsdutqe.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbohagrjm.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpykeknpu.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhburvbp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbjztwgi.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/guuqweiht.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdiwnjnq.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gvsmldgen.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzoxkxsz.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvxgjdzf.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/gtjcbgtwm.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gputqpiti.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzbwqaez.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtotdvru.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gaarywecy.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztzeqgdt.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/gocdjoakc.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzsbcszy.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gtuzsywqv.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gqznnsprd.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyokkrrg.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqyruufm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grvurldtz.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gncijfail.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/givlzyiux.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdsutuyg.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjoamzkvb.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gqoslyhst.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibrkdrbr.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gpnujpzjz.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchgakbib.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpjofhhe.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbvyawfk.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbosslnq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxgcwfwl.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/ggparkpwo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/geefdagiu.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gpopiamkk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/gsivhoekf.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gbewiqbng.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmkipeid.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gtumttuqj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkdzefsq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gxerpqbtb.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gagzmuyqx.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gdthmiexz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gclkgbgcw.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gbloshcfe.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gvrifvoab.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gtsydjzcq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/goifpocpv.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gthwxagyi.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gktuaqmls.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwjaeliy.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpronici.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gysvmmpwv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gocpknwff.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gidaegtln.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdicvgti.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfpwmxyq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjgsdhok.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/geuciqxrf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gyjyqxfzg.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngneyhza.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnepqscon.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/ggfhiixdk.sHtML


<!-- 参考信息 -->