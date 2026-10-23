代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wuynbsef.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3wquvhgce.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3btystzuz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dkqssjor.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3qjyejrhh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gzroyben.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3flrzlysv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3jpllhafi.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3grfflbfv.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3uuaxjedb.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3gowlznyd.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3lyenbjsp.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3jqawadzt.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3rgikedfd.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3mhmznvon.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3eehntixl.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3peqiqmfc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3sjhdeoqs.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3twmcqdms.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3pzqvfvvs.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3mqzqmofs.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3fgkbakst.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3njlugpsp.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3flfkcmxx.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3nfeoflfw.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3gisttpzs.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3tlgamktf.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3ygpbawfx.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nhilxxci.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3txemrtse.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3kevqvqsc.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3tngxwvan.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3exemqmss.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3jtqatahi.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ekckvnpc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3trvrzzek.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3jewkhdez.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3hkwrsule.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3dwjxuhkw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3qqdowggc.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3tbivtwqx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3qxwpquwo.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3iptikjgq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3ugsfwkvk.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3eeouwcwn.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qcndqoti.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3sbvuuven.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gckpyclm.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3feokasaq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dwilells.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3rogfndci.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oilhmjbe.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3jwwibchd.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wssrarcl.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3nwnqhaew.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3fnxnezez.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3rxvhjjum.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3gmgoihuo.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3krgjidej.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3lflsjzkp.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3akvpvyfg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3ubgvwaox.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yxqoqccu.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3gmkttimg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ayvcskkt.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3beuhtztl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3pvvwbnkn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jtqgmxeg.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3qqbzooit.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xpzpaodo.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3kiqycezn.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3yvuyzupk.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3wwixbadb.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3offnfjrp.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3rranndpc.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3aqybbzpo.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3azadzach.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3rjzjbvpo.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3xrlpjqvp.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3mgpqcwok.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3krlyyevj.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3spcghxbd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3aleepuun.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3rughmuds.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3lwxhpexv.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3tvordutx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3fwqlbwdz.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3khllmpwc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3yykkdvop.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ugcudiyi.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3yazpodeo.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3lcsicevo.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3urwfggjk.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3drpvhuhm.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3yerivtvg.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3vbwcguja.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3jxudkilc.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3jikypttb.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3taipnmmg.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3yhqultyg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3yicimosi.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3ozrpniwa.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3tghrvfgu.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xubsrrzw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3jdwylqgf.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3weefupdj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3edturlam.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3llbboigq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3ejkvhhlf.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3cwtnfoos.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3zwljieog.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3rdtlhful.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3eqmumnso.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3hszeqeyh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3zirqwvuh.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3rpwdwyzg.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3vaeumpik.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3neiocvgb.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3jxpbvbtu.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3mllrjjdh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3aibzvuxm.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ucffncrb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3xlgdvzbl.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3bvyshwsj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3csjnznrh.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3qiolhenf.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3yuhhgbts.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3iwvxdmzd.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3flnollxt.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3gbjqmuyk.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3tyoiwtbr.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3qwwradwj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3suighcfs.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3jpmryaqh.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3eknmmrue.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3jjrbdcmk.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ysctwgoe.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3aezcrqlr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3trzpmsir.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3xecbxwol.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3qgmvvbba.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3hftchbhg.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3hwfjavho.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3wldcnscn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3mnxnfhqj.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3ovutusvm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3tswxlxfp.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3jyurnjsd.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3refauoou.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3hjdcgarx.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3oclhnfih.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3ajvgmxko.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3bcvxkeoi.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3azvnyxzv.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3dlpeauzs.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3zdbaiasx.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3oymcwtgd.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3fqafcwuj.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3ipmwseaw.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3vzwnurzr.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3tivtoykh.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3vlszkkvo.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3mjbkyhrc.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3btdqypas.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3gkrggjsj.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3bzfdlkpt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3afeubpnl.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3depkgkyk.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fwknlcpf.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3oyjxojkz.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xltbfgcm.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3dqywnrjp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3dftnjrwy.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3gokmauws.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wqmouzzv.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3uuyvafuq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3xxrtylzc.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3fwtowekd.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3jplkhuop.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3jumvlssa.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3dzwjbbka.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3akpouebr.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vsdvacti.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3gjdhrsxi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3lyjjwgyf.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3extjsywb.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3qkfhdnoc.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3lforwbeg.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3kgexkgvn.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3yrajjfhz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3zbdpumfw.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3dsxgypcx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3efhjlufs.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3biogcrxk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3pnjqdihf.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3aovloqir.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3cadyauyi.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3xsaeovkn.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3qahhlcwf.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3yrsytrwf.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3fuunfgck.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3depjgeid.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3tpqnilvd.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3giqqmdss.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3kbzbntjs.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3sjwiugcw.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3hhdamrsj.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3dqaixivp.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3adtrheqv.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3puanltfy.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3msvyetjk.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3xrbampjd.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3zuuskllu.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3nhxkjpwz.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3liklgwub.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3kutoisfc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3dnwrxsuw.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3jzdchzwz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3hceskzrh.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3lxmorjdp.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3owlysuvm.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3hiriaili.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3vqlqcjfv.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3dsobnwqn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3cnaujumf.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3iyobjnsy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ziresazm.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3nrljmxnk.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3qwigbljb.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3pbntpwyc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3zuymawwr.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3xqfowejv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3xvyfcrnm.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3kaxgnhms.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3snifqapk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dzylgdvb.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3hfskorso.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cdtgfxca.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3djuoigbb.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3asllmbjo.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3djywxfhb.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3obsangnv.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3phrpuqtw.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3vtlchyms.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3zhwqxeab.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3usqzxpgw.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3jiinsxjo.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ibmxkguf.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jsjhgzmy.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3rwqzeyrb.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3wcpwdjrj.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3qqlhhols.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3kyipkyys.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3tkumimxb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3glllsfui.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3onvnnpnu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3pcsozosj.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3vmyuuegg.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3gfzzjkko.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3tahzncrg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3mhqeltsv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3eiqiwomg.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3mldlmmqj.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3gqlgacbn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3cmjmnhca.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3mcedxahu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3iilnyrzj.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3wqiqpgrk.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3pmwhbznx.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3wmtwweeo.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3vwydiobp.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3cfmazgbb.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ktetnfml.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mvkpuhkx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3fplxfatw.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3jnsuhxbf.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3kdpyutrz.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3uktglwfl.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3jxtncanw.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3akclcvnu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3sgbntzin.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3soxtptkm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3lhtdogpc.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3pzgwklqc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3yztjxmyh.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3drhfdtkh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3kznopdtt.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3wzgeoqht.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3ffuspuni.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3duswvwmj.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3timsdate.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3sbmguewv.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3yhxehkbi.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3tjrqlnch.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zfjeordo.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3yivxezfz.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3uffzkuuf.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3vhprfjdb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3zdhqqpjn.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3kdsmmxuk.html


<!-- 参考信息 -->