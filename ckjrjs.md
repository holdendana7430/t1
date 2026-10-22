代发 wailian999

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2whxitugo.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hyaydkrk.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2ljudpjyw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2kiocyljm.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2revtzplt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2jicxqztn.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2oxjgqbrj.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2zavcyjkd.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2wjikkyqt.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2fjelqmvu.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2gfupxpsy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2kteqzagi.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2dlwsufpz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2gubradjq.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2gzruocte.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2snhiibwy.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2sprkmqnf.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2cgeccqxq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2xshslbwm.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2tgiazvhb.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2vbnqdyur.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2pzkmowwp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2gectjmpp.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2zvhecgwa.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tsuruqbw.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2ipmirwyu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2ijnyrnnk.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2dpbdrlbx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2mafexbaa.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2piuddbdc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tqtntkkm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2czyndqiy.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2vaygvqyq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2tkuaxqvp.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2tlbkfnud.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2zvigzqco.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2jilplybc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2qsgquayl.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2hzbwvrby.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2dqdnimtr.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2sffbmpog.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iglxvbmo.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2oyacbpic.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nmhqgbzl.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2xsmdczdw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nzzqqesb.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2odkurewk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wghnwjai.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2xeoiuttz.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2aiprpmjc.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2zjksblgt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2ivufbuis.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2siczcnou.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2hotqirgs.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2gwtrnbam.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2dxmijmst.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2inmtjoax.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2qfshnijg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xwdeejaw.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2idfrifyg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2ssijgjbn.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2knyzilfc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2xcykjqoj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2akwimdim.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2ebqtypsm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vvpcuybk.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2tupzzxrc.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2ratnjmdi.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2daxlgzsg.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2nfsecrnk.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2phcdlhqv.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2sqqetxwu.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2exwetdme.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2qjwtvgln.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2rmhdhmpg.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2igmudqfg.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2ceglrshs.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2jbkrwaqa.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2tfnufgte.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2unhkbtuo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2yrvuqdka.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2azgtduba.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2nsvttxxd.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2qxgdredz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ptbhckvh.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2zbndqtfh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2urtpeoqy.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2qqwrphkp.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2gxlzfibw.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2diqrmavy.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2nefvccux.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2nxivxpvg.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2xdikcszd.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2txfxeuce.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jreyfjce.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2uqtatkqt.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2pvpdplbb.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2iumtqhpk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2nijyebdc.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2otjtyjci.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2ivvkoocs.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2laeomgco.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2jtpjpotk.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2lbfqihxu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2rsnjoygh.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2ueyjcffh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zxqpbgwe.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2lwvtgnhy.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2lsvcfzhg.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2xtkngrjf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2eypwlran.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2szvwqrdp.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2bjceheuc.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2oplyjbyp.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2daoajjht.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2tygpcdjd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2clnnqscn.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2rnypvngo.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2vdjrurfj.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2tddbicld.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2pchaimxc.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2tbcmqkoz.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2ydbemlkj.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2hddzjsan.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2fhzdunmd.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2vgyidjea.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2gelajuzn.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2nehydgkg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2jyvjakfe.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ounvqfno.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2jczjdxjq.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2slusdcjc.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2twqytrfl.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2rurxbtck.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2shjeeowf.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2amkbzllk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2obhclzun.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2fbfiurmd.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2rxpvwwvg.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2rrjicfly.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2fzkgvdtg.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2iueecell.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2vrknkxqg.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2wediknmn.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2bwruypvc.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2yihacsgq.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2nfmwtyzv.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2utlsacbr.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2qxucipbt.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2goccepca.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2fabocwvd.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2mhnwkuie.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2knevglzo.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2liwnmqjp.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2yvogewdo.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2jnrgjvqy.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2uzhhnvpw.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2fejwkphi.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ombukljg.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2dumkeiiy.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2ftivcyhm.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2opsmgnvk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2ymeqsfpt.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2speohoqm.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2gihebbpl.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2hcblimrs.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2svyetsjc.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2xwoosadv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2durscsty.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2hmtzcplo.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2vrygwxtj.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2nrkejmnu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2cjimvgmy.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2jmnuyopc.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2eidfycih.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2rxjqflwk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2ajipxgjx.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2hngppkib.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nbdfcbky.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2wlreilfp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2nkuzdmzi.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2kvlwjmga.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2kgnsyspr.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2hvwvwgal.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2vcrkwnhv.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2xanaxufg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2mldgryeb.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2nysmflby.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2oettjzjr.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2adhgrvyy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2jtwevaja.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2dyavzcea.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2xqqbqwlw.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2zhzbzuob.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2kofwkegp.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2fqbvogbh.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2vkazgmgm.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2wxcqedkn.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2ggnkbanr.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2gzszelgd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2wziroduk.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2npjkktoh.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2gsgvjlgl.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2jylfrqzr.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2tzoybvsb.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ctnuzign.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2kmrnvxjv.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2ifuwtnzw.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2gnqysqpf.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2uxvbpkap.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2fkrfvfuw.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2icyhuqfv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2zlyrupcm.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2cdkqtxsn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2mcxpakmb.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2xhuddtkw.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2toqfyqcg.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2myjnatpy.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2fbvrgvmn.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2miiqhjsv.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2euemrhfo.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2nahdzdpr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2fzojgimh.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2qugvqnbq.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2rkcgjzzb.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2cuqvnddq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2mumtamev.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2eifnstuq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2nnsbktuk.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2uuhbqxbu.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2kzpzlwfp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gpzrlspf.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2owqtrgrg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ywfstquk.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mqwdiklp.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2ybvhtskf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2csakofdl.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2guweorwa.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2cxevwkhz.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2qymbpdqf.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2vzwuapfx.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2djsulgrq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ilyynqcr.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ntbfgmhi.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2sbjnrzde.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2pwqblilc.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2xjosjnyi.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2wxznmscw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2neqqrugs.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2dpqyuybp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2omlvpafz.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ekfwrkqm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2ufmqyheq.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2fuxtmnpc.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2rkchnthe.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2gaedxmts.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2tzqwgihy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2iusdyfef.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2pgjvkver.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ikifprpm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2vspmlplv.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2xembbprg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2xuntbudd.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2kxptbxve.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2togkicic.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2vjvwayrq.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2pnyfygam.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2ddiudttd.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2ezwwynmt.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2cddzqhid.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2mwjscwyf.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ztupivir.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2yhuzrlme.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2rnqobyrn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2rtuacknq.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2xixyyycv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2wtssnicg.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2wgguamrc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2gbxbpxtw.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2eurfaper.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2piqahapd.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2jnfdnkie.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2yyswxnvo.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2bndjbilk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2ufelxncn.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2fnrmklbn.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2kgflhjmn.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2mqkfglcb.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2yzycndup.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2iopcskji.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2pfeicmyw.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2qrglnlbc.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2onpkrilh.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2akoyvfhx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2zitefdmu.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2bnwuybvu.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2hujtmwun.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2ejyljrnp.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2pcrxbwbo.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wajfaneh.html


<!-- 参考信息 -->