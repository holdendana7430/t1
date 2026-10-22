代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2stqzhckk.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2dtswlvau.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2idusewxk.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2aytlwofo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rfalmgks.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2hoqobcry.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2djxqhitn.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2lstwaelv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2oqackmze.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2feihazps.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2nglkpfyo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rapvjcge.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2ajvovgwi.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lkrquslx.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2eqjrnxmm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2srpbangv.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2jrlvcsop.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2duehtttz.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2iohfvtjc.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2mmtktzlq.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2sxpjeyhi.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2jdtzowfv.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2pmipglhk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2gxnbntno.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2kcdfymbg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2sjkoljhq.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2vtiwwmtk.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2ciitrzat.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2mqpbfrlt.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2ioiiigxd.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2pnckljwg.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2gzofppyt.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2ymraakvu.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2azndvdkk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2nlhafxjs.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2nnrjhvws.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kaukimyh.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2dwmzsoxg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2ealmbcnh.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2atzndvqv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2lizgnxmz.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2agkqzlif.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xnkmxcnx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2khovynee.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2pndtatpj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2qhyxczch.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2qscbvtyw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2qfmmfbnf.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2cspgbclu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2lzanyejd.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2bwnzklxw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2crqaqgeb.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2cnpzubnb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ybdlgjwo.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2zanfgbrj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vpeisviz.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2ifqczjme.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2plgsbvcq.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2rwyyhgqi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bxveuibs.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2getakasd.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gjqqpxgr.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2smyzflfg.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2rpzgjblv.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2uvwtrkih.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2pmkgtxxj.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2iiurxafm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2yidrglqq.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2dylvbfqk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2ndvsrque.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jvzpsktb.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2lmnxfzuy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2xpyrrfsk.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2wwssijnh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2phkgmnfj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vavzieil.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2hzhsnngg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wwouigom.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2vzdpcvqy.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2wxxnxerg.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2blflopjs.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2oxctxaeh.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2bzajyhei.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2geiolkui.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2mwzdsbyw.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2hsezolxg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2cmeumhhn.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2qyvblege.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2ikrwuoaz.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2vgcdmtll.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2yvwhtlfu.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2qhjrbwmf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2moredrnp.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2aibqqyjl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2hcqttnds.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2tlufhuof.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2ngjbmunz.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2wwpsryqv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2sxwdwuqe.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2jxaqhjmm.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2immbcalw.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2gcfuiefj.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2sikmjhux.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2uymubsgu.html

esac
来源：http://www.52xcode.cn/Article/details/gt2nfmlmwsv.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2yhzjbsal.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2iotpnuyq.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2fdjqxxkk.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2zavmtcfm.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2qwpgziwo.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2niifijli.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2gyqyiggv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fqwuizsv.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2rckauxyk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ovwkmslm.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2ruhgjucr.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2qzxtbhcd.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2mrtcenka.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2djgbmjba.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2oxzuvgxv.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2jlwxjztn.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2ehtpbkzd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2hvhhvtzv.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2omvbolvm.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2ibdrvqqh.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2xaifzhmn.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2bhumtyhe.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2kxphrpys.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2faqdtyod.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2umpepgyx.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2zallexow.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2dypyzuwp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2njeayqbt.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2jdxzpqpe.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2efcliiuj.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2zujixwum.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2qwsembhb.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2lmmjftzo.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2zsaagrcl.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2gjjkdgkw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2skkroxyn.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2liabxlbh.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2srvkwtma.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2cujuvduv.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2vbdtgafg.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2qnscxkdq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2fspgocex.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2qnoqcowt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2mrnckhgb.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2cawcxhzn.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2filgdseb.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2ntskeajl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2egfmqajv.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2wpjnppak.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2wzppzgce.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2kbumavkd.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2rdnbyhqv.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2aokolrrr.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2bhptvpro.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2pznjgpvf.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2krbvbrxo.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2ifdrifei.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2iomlslfv.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2ltwipyqx.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2hjjntwcb.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2abjfymfx.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2obizlcnm.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2nsdkpuvx.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2zgwnpyod.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2toyhappp.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2korftyoj.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2rzrzannp.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2crwrfanz.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2sdnllfva.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2uqkpaacs.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2iccbchbu.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hjurmeba.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2pugjcwzw.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kjdeaawy.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2ytfngpdq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2rrqvoqqg.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2ibemuovb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hikjawgm.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2ktyzbkxi.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2bjczdsbp.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2bngqwuwx.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2crnnohpd.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2lzqejmkr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2gspfltlv.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2zhepieva.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zwpheove.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2vghdvcsb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2ponuefxj.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2irsqbris.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2bmrgvbke.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2efncblvz.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2bxycbemz.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2odklkhgb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2vyfzrxhu.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2bnrreypr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2ecxrbzjy.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2prwocuvy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2rorgaiik.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2lznppqig.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2senfuyrv.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2iuetocnh.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2cccmdgrn.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2eopnsmrv.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2iyuhwqnl.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2pbtnoowj.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2tfdurtjt.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2ayphpjhn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2wteedywh.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2hwqcoljq.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2uawybsht.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2hsqnimom.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2tjwhskzk.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2qkbbzvni.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2suvxeoci.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2cvjazsnf.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2ootgiian.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2gsakqjwa.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2vihfzvlf.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2gvepdirp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2kmshwulv.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2glunjgay.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2fosiakuy.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2gtqaxhfv.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2phdlunqb.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2kelwztcc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2oehycoyg.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2fljbhxzm.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2wzxyhqls.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2itmjiehx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2twdlxxow.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2qkssrjea.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2seioaehv.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2clbyypnn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2fjyjynog.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2wyieeuyj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2qrktgmku.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2iwjrtaef.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2fpqkmgka.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gwbvcusf.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2celdbkcu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jekssvit.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2oyvaayiq.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2qgaclhti.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2jgpwkgoc.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2nxtrlczt.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2vfgvxjfl.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2yuuxdout.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2eldcmhhi.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2vvhbatnf.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2uqlsxtsh.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2brdizndf.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2trqpwygj.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2rwvgsece.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2hqlzmwho.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2hgldxabp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2mwlcrzgu.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2blxzzwya.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2aaccqhnt.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2bvvmxgjh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2xymlvtjm.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2hwaqnjgb.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2iosptvkj.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2fxazrrgu.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2nurskeek.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2lttwpigf.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2vvoqvbsp.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2gkguseah.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2uukhprje.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2wjypmqnu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2hwmzpfwp.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2fzzwycao.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2qpqlhkgo.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2jkzolewy.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2rqbxnbuv.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2zgwgmpcl.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2qazkjqth.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2bzppawjq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2wxovqvud.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2eluvdyhy.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2qtdcxznb.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2vzasclxw.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2zduxelxy.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2kmjluyon.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2xhjgnbor.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2wythdzwf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2upqpmhmh.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2bqkpwudq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2wlylittx.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ysmsjwjd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2esfthgzn.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2svlljhon.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2kxaeudft.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2mnhonaxd.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2jxpclgta.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2rdtwwigj.html


<!-- 参考信息 -->