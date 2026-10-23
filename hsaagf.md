代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xlripqme.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3cvyvoqqw.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3vtovjfvz.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3yxueuaks.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ewbvdgfn.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3tguruxjx.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3ctpaxywl.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3barxdlgt.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3pgwjdtka.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3kbzjrlkt.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3snacvotx.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3clyjqizf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fuqmxuye.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3gjdxzqbl.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ghotrmgx.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3vavbucpy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qdrtymep.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3iwozdlsg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3kpndectb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ynusjman.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3yaypbuqt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qopilmzu.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3bmomevrw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3kdiszevs.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3qvaqaqju.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3noeupxoy.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3taiwssqv.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3jhldivlh.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3pxwnabnj.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3ffucdyia.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3ijeelhup.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3ptssgaat.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3bippwsdg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3qxngddpz.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3kaoinhqr.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3ocliuiga.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3cweszzqa.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3baviaiqh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3mcyvqyjd.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3hnccvvfn.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3iyziizqx.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3dhvxekpo.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3jokvdscj.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3qkycdyge.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uqzkudfi.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3faungddy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3kjrulzwx.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3ukxkzvre.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3dtgmvzsk.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3oyzzfbby.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mkjmbuog.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3azwxedmx.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3gvluhula.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3vwpdzdtv.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3nfewldqc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3oroaiegl.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3zbafaadh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3altivool.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ugicuamb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3qyepmwhh.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3alatcmid.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3unulpefk.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3xiqtuzik.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tvijwryi.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3tgthofir.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nedpguwk.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3shfobtmb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qjqyswgc.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3dlnpjost.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vdwkzjns.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3ogbizikl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3xkdngpki.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3vuaretjp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3hcjomqji.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3capdmked.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3xuavcwms.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3dwajzinv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3eiqogoay.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3idljslkc.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3xpzjkuyi.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3bbyaigzg.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3wqhcrmvf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3ajnrvecm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vwtifydn.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3llveoxch.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oqynoypj.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3gktnjtho.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3zmnwfnlk.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3fwxviqsz.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3nexwqxil.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3hummplnj.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3hllpeepj.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3wmwujslf.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3mfbobjey.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3vgxfzipp.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3sqvqbicg.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3eslkjluk.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3odfcicct.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3cajosltg.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3wknxsjpj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3phrturfv.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3qmfeqnjb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3xphftzyz.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3wuivezmr.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3wajpxwuw.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3xblorzmp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ogncqkxn.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3ozkxhmfc.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3zhwwmqgj.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3lpqkfqdc.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3wgzpxagn.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3zwfqhyhf.html

esac
来源：http://www.52xcode.cn/Article/details/gt3xcnhpptq.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3kzhezpwu.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3mxfojojm.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3zllmcgna.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3idscndcy.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3nzuxqkra.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3bhvvyaum.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vdnuufsb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hqxqoesa.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3lejbfusz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ldnzbrwe.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3nhsdvnye.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3gizbqpow.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3rectdcam.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3pjjuwxnu.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ubfvevjs.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ycrrxzqj.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3cuuaadzw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3ybechqpo.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3wvyosnfo.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3ffnpetzy.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3cnvgphem.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3yzmbqzyy.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3qfedvlym.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3biyetbhp.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3nncxwezh.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3objqghop.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3msejyywe.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3rkuhmaau.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3hikbvhud.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3hpdnfnpy.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3ncuuynkh.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3eapzwfpz.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3gpwgahge.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3mlspfbrg.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3xycuecaw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3kyrphngm.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3dxfjrwxi.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3qnkiudbt.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3vllztiul.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3lmkyzoeh.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3wgoqgneq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmdcsewo.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3sgliwxnl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3ggotthuy.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3bifolusk.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3czxtotjk.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3goukrgtp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3enazeqne.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3uvyroufk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3cnelxrdg.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3gcelocmv.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3fsqpbqjj.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3jsplpuzv.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3qmsegxqi.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3vucpuilu.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3xqclvzld.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3qcfioqvh.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3hphntiin.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3wsuiypri.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3cqlktwlp.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3urcxdanj.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fvuajjgj.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3tpqgajmx.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3rhnnuqoh.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3olkcquxq.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3korsueyw.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3yxjoluwf.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3iedjrhft.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3crbdjwkm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3ofovpigx.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3blrykpnm.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3mkqhyhfk.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3mqlzmadm.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uxjppify.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3wigfozoe.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3oanqcpgl.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3pnuktkan.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wqfoinwf.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3hbrmxrpr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3qsnxcrdw.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3pvahhrbi.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dnmtedqz.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3xfhgvama.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3wacgjozf.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3cisqjggt.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3oqnxvlcw.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3tkptmwru.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3xkdxirpe.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3yqqjgwqk.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3cbisaqsw.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3fsedexsc.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3rscilgtx.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3honfixxk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3pwizeeyq.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ltkbactu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3bdygilvp.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3imbzldij.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3desipnud.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3mqagkcqx.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3gtldfmvt.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3ocvnyujn.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3vzvtwolk.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3hgraqdbh.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3ccxexylz.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3mredftvs.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3dceciugy.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3rjcewpfd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3ynkhquhn.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3snrfrkbt.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3exzygmll.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3uwgvkoze.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3ehenqtbq.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3bnrqdunj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3iakghdxa.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3drrfggtm.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3xwfyspxx.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3dgttkvuq.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3qlxayueq.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jmxvsbst.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3gczcqopz.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3grhavqfe.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3tznckeoq.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3qhdmldxi.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3gnbscyzt.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3pyyqosve.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3wbreiuhk.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3euuqtvlx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3lhitccrm.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3myscboye.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3xxqzvzrm.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3mxeiwobg.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3zpwkcdyf.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3vuiksdpg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3kijpvyyj.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3jtecqwlo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3tqphxjnj.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3hgzdqapz.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3ctfgcsbh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ajkwwsjg.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3ugycgzey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dcidfnea.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zldywlsz.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3dqnclqod.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3kkjaixrp.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3pueqcxqh.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3czsavppf.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3laucnhla.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3vynirpbj.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3ywvvftfo.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3zvwxihmr.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3fwzyhojz.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3jphpokvl.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3gfwnqnyq.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3tctaccuy.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3jnzkjayf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3gniehpbo.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3uctuoyfc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3zpqnjpzv.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3dkkzjezn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3qnqupanb.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3pfhyqgpy.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3apuwiahg.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fewxwtqe.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3dfkqtmqd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ailftzeg.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3dbzfcnmu.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3wbauljfv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3gvcddtfy.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3rlsyjwjk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3zbtjwabw.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3yiknjeeb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3xeatbbrp.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3yikxyihw.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3bykdyysm.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3rwccgecg.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3rupfadpp.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lvmqpfet.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3eztlclov.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3wosplrhg.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3nrmklrud.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3hedbcaop.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3slhjnfwe.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3sejszinr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3yjyonqfd.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3zqxamjza.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3ykvksyku.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3bltnxfcg.html


<!-- 参考信息 -->