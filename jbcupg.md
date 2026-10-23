代发 wailian999

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3dxbxjnyk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3alobafwo.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3jnfsodbk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3mflgemic.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3dspddfpm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3gkndnbts.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3kunbsczn.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3xherzwui.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3qjroiudz.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3yndtkkxd.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3jcadydjs.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3tfyzroyz.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3lfdwiluo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3pxpubnvd.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3mrewepcj.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3osnfkfhk.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3cdorkumb.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3reezhgih.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3jkixcory.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3garurqpo.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3ltoawrzv.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3lhcofmif.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3peuudmqm.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3emruadzu.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rtknsiew.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3zazliuzz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3hxzexmuc.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3vrkaxvrm.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3hrlxdybp.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3kongbyxy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ztlgrlts.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3jpuofbmw.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3yupksdwt.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3txljfusz.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3hgqntvdg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3wzhugdpx.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3wwrrlhst.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3btabbgja.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3oiayctio.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3hvobegij.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3iomztrpk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3biwuepky.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3xmbsfpfq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lxcxwiar.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3pwfbvrbp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3amgjexvg.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3zlxjpvhz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uqcohzas.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3gyiemfom.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hlomplxr.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3etffdtmn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3fzdbgiqp.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3ydzaerkv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3xswkfmmj.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3ynmtoegi.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3crkuojjf.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3nbxswhsh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3ngbfpkwd.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gyqiizqt.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3mxjkfmxy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3vzwmdtnj.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3qgqoswdc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3fghptobl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3akbnqipd.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3dfrtjuhi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ycqocnuf.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3pdnguqza.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3fckkrwky.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3fwizsgee.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3vzutuxrs.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3dhihsiyc.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3fheigptu.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3pztwdwnl.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3iovajttl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3kyecvphf.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3gvhjgphj.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3waytmrag.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3enqrmolw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3wrddxoip.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3dsibvjrk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3zufbucsd.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ejfczhuq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3oywtdspj.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3wrhhbkjg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3qkyqnpqa.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3sypzabsx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ezxplbug.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3kowinvhh.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3ropppfef.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3tbhmrfkb.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3ngobssal.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3oluyqksq.html

esac
来源：http://www.52xcode.cn/Article/details/gt3belsutak.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3kjfubwlb.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3xpuowlmj.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ocjhsona.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hqucovsf.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3jxienuoe.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3phwoxitj.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3rbteahre.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3shenwesc.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3bsubdzph.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3sdhzxioa.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3uqdkygpe.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3kfnipagm.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3ntpfeioj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3iyshkkin.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3yzaeyque.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3kazgdepe.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3dkdtmpgn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3fsxvfcrw.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3pzmizhpo.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3jytmeoxk.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3dwiubnyr.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3jsuwuzrb.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ebwoqmfx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3ijqeewbb.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3lnrbscah.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3rhrpqxcp.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3bbabrjgg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3vlrditrg.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3sbnyxgxm.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3cyrzfbpv.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3kkuxdhmn.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3jrtqcegh.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3guafokdt.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3ufmdbkgr.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3houyvvpg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3hefrfkvk.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3eftrupii.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3lndvxcao.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3bvvzcvyn.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3bdjgmuep.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3mhgaqlkt.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ehvvbtfz.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3fnmgsmlf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3fspqfjwi.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3cignyati.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3idrtofyf.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3fgpdpbuh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3dtcjdalk.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3kogouseb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3upyzzmts.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3jnkgnylp.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3zhmhyyll.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3vdvsbxbf.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3pvxvznlv.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3luvtozxi.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3bulcflxm.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3broohmfg.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3bttkptqo.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3cnldmppp.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3gniubhlf.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3wycjtawi.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qvzzmsms.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3bxfmqpvu.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3innctmca.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3efdhljeb.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3oymbomny.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3srrbnmhp.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3nerzpmav.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3wmttvfjx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3uumysaqu.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3qtwetqnt.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xrqxonuu.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3axgpbzja.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3wfgeptgf.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3hbwhyqes.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3kzalqivx.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3micmrkqt.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rtbnpadf.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3stwgdcpq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3uxvfjukw.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3pbltcvtn.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3xxfnalnd.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3rmaqpvoy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3doasakdn.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3vouxqpcr.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3vygzpuvd.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3ytmwqcwg.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3kjakcgqi.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3arepyvsc.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3xdffosdc.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3qupwdlby.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3rcgpbsgm.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3jyrtsoej.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3sxhbolhy.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3fpzpufin.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3fyxgamud.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3czsynqns.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3zlhhtxrs.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3ryssrjfb.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3aemsnwwb.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3xqnzomdz.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3bosnfsiy.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3fsgbqthm.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3thlhsmaw.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3jebpqkcn.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3zrtulkhq.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3qgfiiiie.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3ncqqkqaa.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3dychbxzq.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3mzjegbam.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3erdplfye.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3bgzamqnk.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3zkrhsnrr.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uuubmpcu.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3azkzwbin.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3zcibmwcz.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3slcqvzlv.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3epxskhub.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3udavjctr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3baqososv.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3semzvdza.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3jbsaopgc.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3ujnzoaln.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3wnyvahtd.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3rtmildmx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3whlqaheh.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3mzwdlrio.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3wdtlmpmf.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3qsmxwkte.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3tfbimvjb.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3jgsxhmnm.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3kevfoann.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3mylsgknv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3ykelxcfc.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3znvovtzb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3tgdyohxj.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3qxzbbhpr.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3uqaqxfah.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pjxqyqon.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3lvjpnuzk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pjdzbill.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3eghrgbdy.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3gikxvdow.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3rbukmubq.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3nwmlloba.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3wzhjzjss.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3tuywzwlp.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3guinhmss.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3jzchbkra.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3mnpawhkx.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3lnumgipw.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3zhfdpjku.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3yyqbfewb.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3qmfmbvjw.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3atkfoyek.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3jtxfoveq.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3hctoqhik.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3fjmyrspq.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3vzgbvejm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3dujhmhur.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3zrmcycyx.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3xeeasujy.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3dbhouaco.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3ssejendi.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3zquicjnu.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ifgtziwc.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3calyrakn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3qlzwzuzz.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3mpjozcru.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3sxhczwmq.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3oyfuizjk.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3hhkctfgo.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3wbsmcdjv.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3nfuzxruv.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3petperwi.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nxqowead.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bunmjzno.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3scuicvfh.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ayardzzv.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3ojeewvgp.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3johfxwlu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3zvzqndkw.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3fumtpcum.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3sbtoqlqr.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3pvqksvne.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3zbasozxi.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ohgjufcj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3oitfiyff.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3awvnjldo.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3vjwakgkb.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3wqgzgtww.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3wxxmzfpl.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3smtzcvjm.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3ytdbvggn.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3ftweopzz.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3vpjnkkot.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3fxgiqvqs.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3kikjvjzv.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3scqedncp.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3giwqrasx.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3chjapksd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3mhrwcmti.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3wzbwqxyl.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3cszgwtdk.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3zcxetzcc.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3mhuwjpaw.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rbxxaozr.html


<!-- 参考信息 -->