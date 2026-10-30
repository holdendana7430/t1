代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.hesvh.cn/Article/details/gkjhxksxy.sHtML

[Q52] 删除指定行
来源：http://blog.hesvh.cn/Article/details/gpcribych.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gpukmwrri.sHtML

[Q53] 按条件删除
来源：http://m.share.fehbvm.com/Article/details/gzqjqvulx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/gqudesguq.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/ghqbqonot.sHtML

TRUNCATE TABLE logs;
来源：http://blog.zdbjq.cn/Article/details/gkzchxqik.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fehbvm.com/Article/details/gidxsnozi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gjwmqbhff.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.hesvh.cn/Article/details/gnxhjkrhh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fehbvm.com/Article/details/gcwkquanp.sHtML

[Q57] 行号
来源：http://read.share.zdbjq.cn/Article/details/gdxvyfjdv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.hesvh.cn/Article/details/guaurapsz.sHtML

[Q58] 累计求和
来源：http://m.share.zdbjq.cn/Article/details/gberwdmeg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gwcsvbeup.sHtML

[Q59] 分组内累计
来源：http://baike.fehbvm.com/Article/details/gpxkeaqnz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.hesvh.cn/Article/details/guvbwhcdu.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.zdbjq.cn/Article/details/gbwqowiix.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.zdbjq.cn/Article/details/gcfskwzpj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gwtsuvqiv.sHtML

[Q61] 移动平均
来源：http://mobile.fehbvm.com/Article/details/goztfrzsc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gdcmdzzdc.sHtML

[Q62] 分组占比
来源：http://m.share.zdbjq.cn/Article/details/gwkzjphnh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gdunjjslq.sHtML

[Q63] 开启事务
来源：http://baike.zdbjq.cn/Article/details/gdclmjovc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.zdbjq.cn/Article/details/glchhvbiw.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/gqzrulnps.sHtML

COMMIT;
来源：http://mobile.hesvh.cn/Article/details/gjmxtdjmy.sHtML

[Q65] 回滚事务
来源：http://m.share.hesvh.cn/Article/details/gktymdwfv.sHtML

ROLLBACK;
来源：http://3g.fehbvm.com/Article/details/gpelmxzeb.sHtML

[Q66] 行锁查询
来源：http://wap.zdbjq.cn/Article/details/gpjqfazvr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/gtjelhblk.sHtML

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/gyjtuwbww.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.zdbjq.cn/Article/details/gxcapghrc.sHtML

[Q68] 保存点
来源：http://baike.fehbvm.com/Article/details/gdavlgomp.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/gxvejmluo.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/guydbezwj.sHtML

[Q69] 查看执行计划
来源：http://m.share.fehbvm.com/Article/details/ghzlnmxgr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/gljbabddr.sHtML

[Q70] 更新统计信息
来源：http://m.share.fehbvm.com/Article/details/glfszwanf.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/gyfkddwea.sHtML

[Q71] 查看建表语句
来源：http://blog.hesvh.cn/Article/details/gcukfubno.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.hesvh.cn/Article/details/gfzcgzpuc.sHtML

[Q72] 查看索引
来源：http://www.share.fehbvm.com/Article/details/gjfeylofc.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ghoctxjfx.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/giimkguos.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.hesvh.cn/Article/details/ggessqlyk.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/glpukeeak.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/gbtykfdvj.sHtML

[Q75] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/ggarrragf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gcoqsbgyk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.zdbjq.cn/Article/details/gjqxxqgao.sHtML

[Q76] 按天统计
来源：http://3g.fehbvm.com/Article/details/gelfkwung.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.hesvh.cn/Article/details/gvsogcotk.sHtML

[Q77] 时间加减
来源：http://mobile.hesvh.cn/Article/details/gajwauimk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/gnebltdwc.sHtML

[Q78] 当前时间
来源：http://wap.hesvh.cn/Article/details/gddujulls.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.hesvh.cn/Article/details/gcajlwbgc.sHtML

[Q79] 字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gwjmlbeis.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fehbvm.com/Article/details/gbvqavofa.sHtML

[Q80] 字符串截取
来源：http://wap.fehbvm.com/Article/details/gsbakjmur.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/guorkbwhu.sHtML

[Q81] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gfwagrver.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.zdbjq.cn/Article/details/gcriyibrv.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.hesvh.cn/Article/details/gsvqmttoz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/grkhuhhuj.sHtML

[Q83] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gdihjkico.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gjmcottxk.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.zdbjq.cn/Article/details/griujsckl.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/goghyxicu.sHtML

[Q85] 数值取整
来源：http://3g.zdbjq.cn/Article/details/geubzyjbg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gnzekxihx.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.hesvh.cn/Article/details/ghodtdmgq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/gqqziheko.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fehbvm.com/Article/details/gdxrqsfom.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fehbvm.com/Article/details/gxvfspfpx.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/ghpwrkakk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/glrumxdwd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fehbvm.com/Article/details/ganwpjegk.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gxcatjcth.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fehbvm.com/Article/details/gzkbxomoj.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/gkirfaova.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/gtiqzmokc.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqetsjewp.sHtML

R. Bash 专题
来源：http://m.share.zdbjq.cn/Article/details/gnrlpffgr.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqlbgkfhv.sHtML

[R01] shebang 与严格模式
来源：http://mobile.hesvh.cn/Article/details/gaqbwcrls.sHtML

#!/usr/bin/env bash
来源：http://wap.fehbvm.com/Article/details/glpzaihrv.sHtML

set -euo pipefail
来源：http://m.share.fehbvm.com/Article/details/gxwstvmco.sHtML

[R02] 变量赋值与使用
来源：http://blog.zdbjq.cn/Article/details/gmsbegwmz.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/galjwipqu.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/grujpsvgr.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/gderfvubd.sHtML

[R04] 位置参数
来源：http://3g.hesvh.cn/Article/details/geoziwifn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/gqkpmihvz.sHtML

[R05] 参数默认值
来源：http://read.share.hesvh.cn/Article/details/gzwrsyknd.sHtML

name="${1:-default}"
来源：http://mobile.fehbvm.com/Article/details/gddrbamgm.sHtML

[R06] 判断命令是否存在
来源：http://wap.fehbvm.com/Article/details/guikafggc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gzeuxrrqi.sHtML

[R07] if 判断文件
来源：http://baike.hesvh.cn/Article/details/gpjppmlmt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fehbvm.com/Article/details/glafnijoy.sHtML

[R08] 数值比较
来源：http://3g.zdbjq.cn/Article/details/ghuyqnkgy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.zdbjq.cn/Article/details/gimpwbouv.sHtML

[R09] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/gubrxbwqk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.zdbjq.cn/Article/details/gzowhuzan.sHtML

[R10] 正则匹配
来源：http://www.blog.zdbjq.cn/Article/details/gdzcuilmw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.hesvh.cn/Article/details/gexlpxkmt.sHtML

[R11] case 多分支
来源：http://3g.hesvh.cn/Article/details/gxlhkmyap.sHtML

case "$1" in
来源：http://m.share.hesvh.cn/Article/details/ggazimjuu.sHtML

start) echo "启动" ;;
来源：http://www.share.fehbvm.com/Article/details/gugvgofxq.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fehbvm.com/Article/details/gitizvxwh.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fehbvm.com/Article/details/gxjoixhpu.sHtML

esac
来源：http://www.blog.fehbvm.com/Article/details/gfussfntt.sHtML

[R12] for 遍历文件
来源：http://www.blog.hesvh.cn/Article/details/gxqkllvic.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.zdbjq.cn/Article/details/greqznatz.sHtML

[R13] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/gbdjrrmii.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/grggsjwtj.sHtML

[R14] C 风格 for
来源：http://www.blog.hesvh.cn/Article/details/gbjmjswdy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/goipoycgc.sHtML

[R15] while 逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gmxnewknh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.hesvh.cn/Article/details/geuivyqrs.sHtML

[R16] until 等待条件
来源：http://baike.fehbvm.com/Article/details/grqvgytdk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/grgirmlfi.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/gmoonabwm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/gzoizpewe.sHtML

[R18] 遍历数组
来源：http://mobile.zdbjq.cn/Article/details/gqettpcmb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/gsglfsncp.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gondswtas.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.hesvh.cn/Article/details/grchohuvy.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.zdbjq.cn/Article/details/gpwhfjabn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gchzgvggg.sHtML

[R21] 字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gsnakyhjs.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/gwfmjnasp.sHtML

[R22] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gqwihqtgt.sHtML

echo "${s:0:5}"
来源：http://blog.hesvh.cn/Article/details/gtxpdoemz.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gbdzkezwp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/gtmtlezcv.sHtML

[R24] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gshavhkmo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.hesvh.cn/Article/details/gbwukgelf.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/gcxnxoacj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/gdyiczdau.sHtML

[R26] 命令替换
来源：http://3g.hesvh.cn/Article/details/gijewnbrf.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/giqvahvwm.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/gakqqaqjd.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fehbvm.com/Article/details/gqwizmgnj.sHtML

[R28] 浮点运算
来源：http://baike.zdbjq.cn/Article/details/geinjvivu.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/gjkjunvkn.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gqaxnrozu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.zdbjq.cn/Article/details/gdpdafqfu.sHtML

[R30] 函数返回状态码
来源：http://www.blog.hesvh.cn/Article/details/gtyhecgvl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/gobiqikxl.sHtML

[R31] 局部变量
来源：http://www.share.zdbjq.cn/Article/details/gakgdtckx.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.zdbjq.cn/Article/details/gvgwplrfm.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/gtrrroozu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gsvypvueh.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/gvnnnaydg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.zdbjq.cn/Article/details/gnbllhgmd.sHtML

[R34] 退出时清理
来源：http://mobile.fehbvm.com/Article/details/glihohkwa.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gbhzmumas.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fehbvm.com/Article/details/grapjglwu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/gkyijfufj.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/gjcoiuxau.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fehbvm.com/Article/details/guzxnehit.sHtML

[R37] 把输出赋给变量
来源：http://baike.fehbvm.com/Article/details/ghojxrifs.sHtML

files=$(ls -1)
来源：http://mobile.hesvh.cn/Article/details/grdtlsell.sHtML

[R38] 管道串联
来源：http://3g.zdbjq.cn/Article/details/ghnecpjys.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.hesvh.cn/Article/details/gulxpnsax.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.hesvh.cn/Article/details/gpiwimrph.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/gfhhffvbj.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gugshflpq.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/ghxvmyrxp.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/gtzyattot.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fehbvm.com/Article/details/glqohdnos.sHtML

[R42] 输入重定向
来源：http://read.share.zdbjq.cn/Article/details/glzbcozsq.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/gvabhvqko.sHtML

[R43] 按名字查找文件
来源：http://baike.hesvh.cn/Article/details/gnpetianr.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/gjoohgfit.sHtML

[R44] 按修改时间查找
来源：http://m.share.fehbvm.com/Article/details/gkjglpkfz.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/gejbykloo.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/gahvmnyxc.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fehbvm.com/Article/details/gohjzobjw.sHtML

[R46] 递归替换文件内容
来源：http://blog.zdbjq.cn/Article/details/gqitwcxnl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/gkdhctucd.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/gnelgsyno.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fehbvm.com/Article/details/gpiougywq.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gjgkmpuye.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gtmdcvbar.sHtML

[R49] awk 带条件
来源：http://baike.zdbjq.cn/Article/details/guerltrwc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/gsunowqni.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/gnfeuxmml.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/guxrgcztw.sHtML

[R51] 排序去重取前几
来源：http://blog.hesvh.cn/Article/details/ggpryxipd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/gtreiqxif.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/gddpnptqk.sHtML

wc -l a.txt
来源：http://www.m.share.fehbvm.com/Article/details/guuurxvgj.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/goadircon.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/gtlbysuyr.sHtML

[R54] 比较两个文件
来源：http://www.share.fehbvm.com/Article/details/gupnvhgqd.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/gmxqorilu.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/gwlaiktbo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fehbvm.com/Article/details/gabvloyhy.sHtML

[R56] 远程拷贝
来源：http://read.share.hesvh.cn/Article/details/garhwefld.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/guayskdyl.sHtML

[R57] 远程执行命令
来源：http://read.share.fehbvm.com/Article/details/gzlpsxidh.sHtML

ssh user@host 'uptime'
来源：http://baike.hesvh.cn/Article/details/gzxlpdmid.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/gdnobgweo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fehbvm.com/Article/details/gqtqbwtlo.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gkoddilau.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/gkxyzscdb.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gdggtlaid.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.zdbjq.cn/Article/details/gydjttwki.sHtML

[R61] 磁盘占用
来源：http://3g.fehbvm.com/Article/details/gjmgrqufk.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/guqaokzlv.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/glqkhlplg.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.hesvh.cn/Article/details/gshtegprw.sHtML

[R63] 内存与进程
来源：http://www.share.hesvh.cn/Article/details/gjwztxjfr.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.zdbjq.cn/Article/details/gkzhxkhxf.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/gquvnesoc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fehbvm.com/Article/details/gcfyjygcl.sHtML

[R65] 查看端口占用
来源：http://mobile.zdbjq.cn/Article/details/gtvxbxgxk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.zdbjq.cn/Article/details/gvhrzwmmn.sHtML

[R66] 定时任务
来源：http://wap.hesvh.cn/Article/details/gozfxxcjf.sHtML

crontab -e;  crontab -l
来源：http://www.share.zdbjq.cn/Article/details/grcenzcan.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/gsxuvodej.sHtML

openssl rand -hex 16
来源：http://mobile.zdbjq.cn/Article/details/gaarhddjr.sHtML

[R68] 计算文件校验值
来源：http://www.blog.zdbjq.cn/Article/details/gwtyidgts.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/glzyugjwv.sHtML

[R69] 生成随机密码
来源：http://www.blog.fehbvm.com/Article/details/gafnyqhpv.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fehbvm.com/Article/details/gfsbexwnv.sHtML

[R70] 时间戳与互转
来源：http://www.share.hesvh.cn/Article/details/gkekllenn.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/gbzqjgepo.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gntndrtlj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fehbvm.com/Article/details/ggdydzgxx.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/ggovwlbof.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gnrsvefgy.sHtML

[R73] 分割大日志
来源：http://www.m.share.zdbjq.cn/Article/details/gkkyhmhzs.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/gnmzwpivc.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/gwmjrskac.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.zdbjq.cn/Article/details/giuqluaqv.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/galnxrljv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/gjgcghpwu.sHtML

[R76] 使用临时文件
来源：http://wap.zdbjq.cn/Article/details/grkjbhuux.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/guujqfirp.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/gtnnedkfe.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/gvsqrvoyn.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/gzjipcgfe.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.zdbjq.cn/Article/details/ggrfsfkex.sHtML

[R79] 解析命令行选项
来源：http://m.share.hesvh.cn/Article/details/ggzknwsyk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fehbvm.com/Article/details/gmjuikmdi.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fehbvm.com/Article/details/glhgltvaz.sHtML

time ./run.sh
来源：http://wap.zdbjq.cn/Article/details/gzchzafrz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbiiolnig.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/gdxcnftku.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmoelpgdm.sHtML

[S01] C：Hello World
来源：http://m.share.hesvh.cn/Article/details/gggwaeobe.sHtML

#include <stdio.h>
来源：http://wap.hesvh.cn/Article/details/gpcfkefil.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/grdxmfhiz.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gthwffgdm.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.hesvh.cn/Article/details/gitorldau.sHtML

[S03] C：读入整数
来源：http://mobile.hesvh.cn/Article/details/gqmrhgwfb.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fehbvm.com/Article/details/grpozafpk.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/gwsqivzyd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gpwxuhiui.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/glvjjyiri.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gpjhgawlm.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/gjfinkjqc.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/gqeznkxps.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/grjkkhnjj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fehbvm.com/Article/details/gaarkazok.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/gbwybbuqb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/gycgwkzwx.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.hesvh.cn/Article/details/gnazgpvjs.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fehbvm.com/Article/details/gwqxaojaa.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/gsdvznbqj.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/giqzywthg.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gblsoiqjl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.zdbjq.cn/Article/details/glbbyyjpp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fehbvm.com/Article/details/guhrgurty.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gbwoudsrm.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/gsdvtnnbj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gakfxwkvs.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/guucjabar.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.zdbjq.cn/Article/details/gmwokiwip.sHtML

[S14] C：枚举
来源：http://wap.fehbvm.com/Article/details/gyxylvmrz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/gwoglkygw.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/georqtspq.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/grizdjtnw.sHtML

[S16] C：位操作置位
来源：http://www.share.fehbvm.com/Article/details/gaayrujwa.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gyotjqlje.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gbcxcquri.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.hesvh.cn/Article/details/gtovhkoyr.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/gersywzzt.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/gtlfjnyhg.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gkwxisfil.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gmayadxhb.sHtML

[S20] C：二分查找
来源：http://wap.fehbvm.com/Article/details/gswocealq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gfqkuymic.sHtML

[S21] C：字符类别判断
来源：http://wap.zdbjq.cn/Article/details/gtnbwgebl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/gezxcuafy.sHtML

[S22] C：字符串转数字
来源：http://blog.hesvh.cn/Article/details/gjjxchslp.sHtML


<!-- 参考信息 -->