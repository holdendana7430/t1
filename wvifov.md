代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3hezebsci.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3vkhvcigq.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3pnhtdcep.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3tmxhvpzg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3zfzykokl.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3pafafblt.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3zciczicf.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3maatzdsw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3vncedczk.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3uavtimob.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3wpuvbyal.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3keeibmru.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yyuralcy.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3sygiypum.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fahuqipy.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3ajoegetm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tyffmasz.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3eghcqmec.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3eouwicza.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vbqtdujb.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3cotrapvs.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qbltsfmg.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3tcypwpsc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ehktdmuh.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3dyvpufot.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3fyiauvuz.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3zjktekba.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3uuaxbnue.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3bfrbqdxf.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3pifpxpwy.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3xkebtaxe.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3ivzdgjpt.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3wmfqsfsh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3ubfhcykg.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3vooxpuag.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3fkvjryra.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3ojdvlzfh.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3pbpqsxyd.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3awfgmgft.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3gjlemnvq.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3hxephozm.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3buvepxky.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3gxabtfym.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3irzlyfdc.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tzumwblo.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3qcibwmwp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3fsppdnkq.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3nrealufq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3mzvjamhi.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pbaakklc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pevjbjsd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3rlqlkdnj.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3aypwitcm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3gmuxjqtx.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3qfpvlezn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3bjaburgr.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3wtokwkef.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3pywfoblx.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3dqzojvph.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3tcfcdkwa.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3fktrfrvc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3weagxfio.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3eziyzhrn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3renqkvyo.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3ycclgtrr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qvygrkra.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3rfxrbjvz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xkjskegh.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3lyddvdma.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yoaajcil.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3ymvoknrt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3fcbnarai.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3bfyuzxnp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3enzdbpqg.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3zogowtpf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3jvzrplmd.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3duqejldy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3clflylyg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gxczscdi.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3fudffeuk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3udtjdqvz.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3gqyxuqlh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3prnsmyyz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jjpkzqbo.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ersyfjbv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rmbhateg.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3rovdlosx.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3xbpyfdby.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3rkydiaxa.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3yyaggpie.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3voeqjiao.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3sbwscetr.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3ejfywila.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3xipiypgp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3lqcxgmrn.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3vwphmfpl.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3yaznvrjb.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3zafvbskq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3nuupdzbl.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3kzczcswi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jgowerch.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3ipgfskka.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3ybqrxqzj.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3rntbcooa.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3arwdocqa.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3npyzjjxy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3fjuiyjsf.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3dblnljfp.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3lfiemrjc.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3txmzeedh.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3sipecois.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3xbcmrzdn.html

esac
来源：http://www.52xcode.cn/Article/details/gt3kymymnpk.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3wtjopaui.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3aolvjnzd.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3oukxwepu.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rikbupen.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3udwjrcib.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rhfdheud.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qxaluwby.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ahdcxlvp.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3dhvyxfop.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3drtgotki.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3cvrbtrbe.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3jpvyuvnj.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3fnyqbuhe.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3tpgxjbfj.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3uyjafzyz.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3clkbjvks.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3ovialsct.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3jjsbugdq.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3zygetyqq.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3ahroorsi.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3amrdmgid.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3ygsllthc.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3wddqwael.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3aiwrzkit.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3macnfntf.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3kwotoorr.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3kppffjue.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3opirmryi.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3cuoudiui.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3jtgljfss.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3zvgehnjt.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3hfssyrlr.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3gydcffpf.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3kmokufdi.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3fglbmzsx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3llwbqniq.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3hydiabyv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3vhzsjand.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3ilhuagza.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qnjunybb.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3cswzssdx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3hrbsecwp.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3indyfrsx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3xjzfyovf.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3tyvhpvdd.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3mglhgvkm.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3rzohtuvi.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3lndvggcb.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3dgoajija.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3wzwpgsap.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3azjvhqtg.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3pvwnqdwp.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3znzfaxcg.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3moexcqbc.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3owneeflz.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3aewbomga.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3manbgsum.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3mfohrfaz.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3cbkdpgay.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3nssjciri.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3lwyjqwuz.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sioohifm.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3higexpdd.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3hdtqtkbq.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3phwzkkkz.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3gcrfsacn.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3mqquuqpx.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3rtvdqvuw.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3xjdqkwav.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3aervpxek.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3pazqhmrn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3usprlfcn.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3hkppddnn.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3swrkpcdg.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3amssgpum.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3wytdxccf.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3yuumrvac.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zvfhbwdu.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3izwjhoot.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3alxpvela.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3elzllddn.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3fcksemvt.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3otzwvjbk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3tllclzze.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3yfexnlki.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wasungvp.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3lmybgehe.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3emnwaukv.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3hsnhttre.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3refqotow.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3prksykmf.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3fyvgaigo.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3ijqoclsu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3zssviuqn.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ukkzpaxe.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3hidghcpd.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3qwolabhb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3flwwktnk.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3nyuwlovq.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3csevjsza.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3nrkdxmix.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3ktljvviz.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3vnzqrimm.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3zdohabyf.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3cewmmjjx.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3rodnzwhb.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3aotcebok.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3vvxvutlo.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3gjthiuob.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3zhfrkzll.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3cznsmihk.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3gxtinmqr.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3covxexha.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3kpzhrbkd.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3zhzxeaeo.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3bytymhrg.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3swneejst.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3vtuvqjmu.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3rlnzklex.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3tpnkwium.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3kblvnosn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3fbztsqaa.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3moqlzmrn.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3vpqznhwq.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3lusdjikx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wynqbwaa.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3sjnfezgx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3unoeahtl.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3nloftqqw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3eidjnydh.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3imztfhmo.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3dpcugsro.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3fnniegxk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3qwiqidgp.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3nubcltyl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3ttvwugsr.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3qwikfsld.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3cmrruium.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wbtuvnro.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3dhpdmehc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ncqatumr.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tsplkwpi.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3nfxaezgx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3duonhzyk.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3xzofdepw.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3mqrpwebz.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3pjwgiqlt.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3syjyolvx.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3pejfjsin.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3caghikfj.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3cmlnbzbm.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3jsbndlyh.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3obzyphfq.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3nittkbpa.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3gedlupth.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3qomwjdwb.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3nvzsjqtp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3anjrgrdl.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3vkoomuhq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3ctshvkwc.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3erzxpety.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3jxzrinxp.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3swisyinl.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3kjfedmxg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3xgezwqrt.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3rjewrijo.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3jwgqhtgx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3uxcogfpo.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3crdrfhwx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3cpdwuxyl.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hifikhxi.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3elrzeauu.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3ntyhiert.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3oxzrledr.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3hfepjjkv.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ykwtvwll.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rbkyaaao.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3xzofhpeb.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3yatxggxq.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3czwvjgff.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3wadxqgoo.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ngkaeisg.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3joekbmhx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3mikzmerd.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3kxnxifdp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3wmryxabd.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3vcutmrgj.html


<!-- 参考信息 -->