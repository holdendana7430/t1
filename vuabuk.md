代发 wailian999

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3dnikvxzr.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3uffdkvmd.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3ljvaztvl.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3sagegvzt.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3zhglezez.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3jaznoype.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3zigylfub.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3xfiwfvbn.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3kadxsizh.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3llzlbtgs.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3kcgygurg.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3bhrwjeqg.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3yzrtknon.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3qajkscxv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3koabfyum.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3lzudiigo.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fbelvhsm.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3illbezmn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3bzefaona.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3uxkljqgx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3lfaequvn.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3czwlxiko.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gocymdgz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3mgqwbdmq.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3qsgxavze.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3egbuyfct.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3gzjuxnfw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3khxcnwpn.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3hcbnkwjt.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3exjlgwqy.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3vfhssnwr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3ablbhrgs.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3wgjzwuti.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wtvvpppy.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3kexlnzqt.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qqlizqwi.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3bkxxyxsk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ftowboom.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3pmuuyxoc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qokjndfa.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3ewekkszr.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bwjwlenc.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3ujngeqgm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3jjxuwkfc.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3qipxtrtl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3whvucssl.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3qabnofsi.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3lwwncvdq.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3fedazjey.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3wrvkoazm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3huuskzoz.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3elhpdqhl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ldpathwq.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3kdpyqgfo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3gqxyclwf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cypfeiau.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3hkpfjgog.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dqtnyblu.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3dkgnhmvw.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3ujiufxky.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3kgqgzvww.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3edwwnywe.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3bggatlas.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3pgtbsoak.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3wuvzdoyn.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3chwxtzlk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3fydzwwlt.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3kjsinisy.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3tbexkuka.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3dxisnhxn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3dvchtkfp.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3ddkrlyai.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3gmaamhjq.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3aestwtpx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3okpxelsj.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3iouujxiu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3zbdxtlze.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3tothfmmm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3zhuvtlqr.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3ssvrabpo.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3txojfnba.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3uwjnylrk.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3whytykyl.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3klokmebc.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3qbqajhrb.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3kbdsotwj.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3aenrkazg.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3jqtduqvd.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3bbtcosgs.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3qfcnovgf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rddctipy.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3pvazrlln.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3obnejbyh.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3xrtqbudg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3jjteesrt.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3clgxvrdu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3bcqvkwxt.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3jfvqvggq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3ncnebeqb.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3puzsflhs.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3uajeqhel.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3vkdxlggw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3lyxmxeoy.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3xpmldxgn.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3vlumczhb.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3fzyxptpa.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3rywvbiqe.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3bapqghvf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3mrvennyb.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3rhsteopb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3rxufrenj.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3surrwvgj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3cjsfkenb.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3zyschheb.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3uqyszagc.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3wrxccyab.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3gyymhxzn.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3oxpslrje.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3dwexjabi.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3qlplozeu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3vnemfxga.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3whtizuoo.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3jqcqowrq.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3nwoovtpw.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mlllkhrj.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3hmfixrju.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3nyyqtbpx.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3kxcqfqfg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3rngctkzr.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3bmzpwegs.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3igkrkngb.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3gbieclld.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3yliblrzz.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3obztcwgu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3izteamyf.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3dqgtgtkj.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3lzppwwny.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3koxqeqod.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3bppqfrpr.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3pnzugczi.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3harfridr.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3eaichbnb.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3dumaynah.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3pmfaviml.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3xlkiaoah.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3zcqwohdw.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gfxpfifj.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3cwlgmjof.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3uoxdkkeq.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3jfcjtebf.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3dzpkcyvr.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3pgdktegl.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3lmiwviwr.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3bpclapag.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3kofzauyu.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3clqzrhos.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mjtacimx.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3tqlvqtcn.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3astlwinh.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3ttkjepxl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3gqygowtk.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3khwjrybi.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3trxlapip.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3zrjgfbpw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3hmxwkxtt.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3cxezjkgu.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qmyigzxx.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3nquxdddr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3xfpgfjrs.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3zjjqhlet.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vuurcwvd.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3euucxyfu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3leosynog.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ymjqyjmx.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3yofxrxqb.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ksvtmlse.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3dwwjkurv.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3ipjikbti.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3gegomugh.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3czdkocyy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3qubfozhk.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3xkgymara.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3wjsvskjw.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3zpvihige.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3fefocsfg.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3azynpujn.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3ypckgaxy.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3jjgnpilp.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3wczfywbv.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3cpzzospo.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3idedfnms.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3uxiopvzk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3uigonjdx.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3ydwrpncw.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3krgxfpkj.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3vikageih.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3jdickjht.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3pvvwttod.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tothoppp.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3wiqysbnx.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3ajtmfrpz.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3kgzdbgxa.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3cpugspzi.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mnlqqoii.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3ivpjnxog.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3rspysklh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3hnajgnxh.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3kqrkmgki.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3pfiniuau.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3omosjxzp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3iubthwsh.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ritglzlp.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3gjazsiec.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3xtwmpsfo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3hqqeyxge.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3fnskapaa.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3nhuhquku.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3zctqliij.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3vxqtojti.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3xupbsxsj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3pugtydxp.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3kgbejugh.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3wvgyaaij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gcafwsrf.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3apdzufkq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kqwdvzuq.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kmmdilma.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3krucqnzc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3raxvaoza.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3affgaccw.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3nvjnqzvp.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3amiivizu.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3nnhfmefo.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3yodvvwjr.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3vbexnpte.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3cvpmzqeg.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nfusisdm.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3qjusqnrw.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3jjykigkm.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3nhkqcyhk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3rjenqbuv.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3jygfxrjm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3mdkhgnom.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3ercgeqxi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3saoesaib.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3ifdrxldu.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3kmbgqrgg.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vcnmzytm.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3gbknfaok.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3ymttsqfb.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3cokplqpg.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3joybnozd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3dgnrdwbj.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3rxxyauin.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3erxmrwuj.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3gxvhbmbp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3hhqfnany.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3pjquqafa.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3ritjjwda.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3ewpqiwrq.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3mpixwyrz.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3lctqzkfn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3fmrarxse.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3xvqmmznl.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3xosoavqp.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3zdginuvg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3epjfbdnx.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3ifzmgqgg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3tivfogqn.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3txzuuxob.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3dxbppxqh.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3zolwhcoc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3ppekylyj.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3tkrnxdgb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3qkdsxace.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3iefmhsvc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3esxqxrss.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3jmogyzfd.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3bnbouhsb.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3xjhivzph.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3kzyrdgie.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3iesbvcyr.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fjtmlfok.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3kaqiglit.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3bmvustfy.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3jtlbwsak.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3ltupcisb.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3kuwakiih.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3mdguqgbp.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3ffmugkjj.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3zybrkqeb.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bbxosebs.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3ggiuoskl.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3jggdxkbd.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ynldilot.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3suqzbqts.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3ltcszbrl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kdkkydrh.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3kkakdpdy.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3zxguvceb.html


<!-- 参考信息 -->