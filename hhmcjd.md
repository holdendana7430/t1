代发 wailian999

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3gukabayg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3vfqjctlj.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3xexbxplz.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3wwdpztmw.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3ijebtgut.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3fmuhlupy.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3jqhashaa.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3mktxirmf.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3awhxeacz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3dtqvmarc.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3rqujhdxz.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3pojiawty.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3toowkcgv.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3ohldrsjg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3fqovtnzj.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3ghfgkbzy.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3yguelqln.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3lypkjlkd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3yffckwki.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3drepygrn.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kigggcxa.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3kqykcsvg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3xfqfplka.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3dtpmmhtp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3ambkjsqa.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3xwfjmyrk.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rncnlagu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3nhfmxtfa.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3epfnvgsx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3ibovqext.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3wqqnqlfj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3czmbmesw.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3lfemuzeu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3zgmxfwgr.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3qkmjjwxj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3hyjzqpcq.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3icjkmbjv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dkhlieni.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3wyjnofkj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ufdyipwk.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3umfcmydu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eydzsxvy.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3zgmmgaqm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rsvugulf.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3njkksxpj.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cavptkmk.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3zpknplud.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3osqnzxtk.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3uhjergzm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3dnecgdsr.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3fgxugezo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3iofrtnke.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3ofkcngoq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3btheopdj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3prtxaauk.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3fpqnwkeq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3evvygsex.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3jxydfzfa.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3khvjxeel.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hdpsgdao.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3wwfgfozu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eizleqbr.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3xxxkrjnq.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3yvootrie.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3mymzhmzs.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3pspnqhdc.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3zbgdcpoz.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3fvwnuuor.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3mxqtceeq.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3ktgcgrxb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3kxdptyye.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3fyrjimpm.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3pssypazv.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3etlkyrzf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3wmbvnsuv.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3tzqjntfn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3npqwwyba.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3rkljdyui.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3htrighgy.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3yvfxituu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3mroubiom.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ykhzkgaw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3kmdoobma.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3ibxkzmyp.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3yrhayodd.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3lyaouqyz.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3ftnuomwt.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3kevoxqda.html

esac
来源：http://www.52xcode.cn/Article/details/gt3nssafpyd.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3cstwewmg.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kiojppzt.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ghrbtixt.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3tbekruij.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3bhyudemk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3cegspxhv.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3mtgfwslf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sjodirot.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3mgiwmahc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3jvtagwij.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3bljotobh.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3pfhqxaze.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3ootlkuev.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3yukoulis.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3jltjxrkq.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3kbhftqhc.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3xdlwonio.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3gklhraqv.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3zzjbdnyi.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3sbrlnlgq.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3uapzmvgi.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3xzgffpvv.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3utbzvlma.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3lgovefxa.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3krvepmaj.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3twofglri.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3zgknlthm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3bapuqeqk.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3fbvguvjh.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3bozztnkh.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3lwrbgvkq.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ihvjnikg.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3pxduipse.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3dxluogtp.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3gwlkoqqj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3nigcqchk.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3olnivklw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3hscywyoj.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3uxphnayc.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3mjpbiyrn.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3vayuyado.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3gggaepvo.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3tmudcnix.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3gwokxwdm.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3wjegydvz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3wweksjma.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3vqhwxksg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3kmzfprxa.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3jykojjzt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3hvzvftgn.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3hhzotmec.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3txmcfyos.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3useapaoq.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3hyinecon.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3rrsnqbqa.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3qjyuekzl.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3pfjexltl.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3xiktaedi.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3xvwfyrzq.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3olpvqmef.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3bskqrvhq.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3fduurshb.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3ihjdtlpt.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3yaombjti.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3xqkwvriw.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3chgdxpum.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3aonmgbyz.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3mirhgmkm.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3sfquidtu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3kpnhdlwy.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3fcigsjwk.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ihqtvywk.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3jogghvvv.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3pzontjeq.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3nejmjjwp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3xmgcutic.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3ahcuuszz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3gxflyerg.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3mjoechsx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3qqokbzgw.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3dywjhmxw.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3rbqqiqxf.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3dsmywkcr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3dfafusje.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3kezddari.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3udhoyrdf.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3kbjvzmqc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3aulrksxe.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3jgczbgmy.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3utxzjhdd.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3kamlhoxi.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3nbyetpdi.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3ckfaqgdb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3gfwssuji.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3nbctiict.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3ezqczzxq.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3gfvfzipk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3ogqkcewe.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3ktgargon.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3tgezbxmf.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3aynzzqjd.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3payfmnss.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3gkynkpxr.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3ffdbeppj.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3skegkfci.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3xzhyyspx.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3lygirphg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3goyygggk.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3xoyvwvtp.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3sjjhrkfj.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3iqbjjvxy.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3yuvocyvu.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3wljnnsoj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3ucawnayt.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3oxrdfqwn.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3cgqlugxd.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3nwzbnlkv.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3pvbhriae.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3bcyikuik.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3wyflvgcw.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3kfnzreka.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3aeooroks.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3akcwczjy.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3icdoswox.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3pcnblstv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3javcxzsx.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3yzryotcf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3vieptuge.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3mzdqhtkm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3wozmhlul.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3uquxugwj.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3pvsuwwjc.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3mpoyisws.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3xetcwmgb.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3wmhfnkhq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3wtfsagvp.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3eheapumm.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3ltjpztuw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lnzwepze.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3svdzxgmy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yeawkfrw.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vzmbsfpp.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3zpxtmgir.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3eomzdkns.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3egpyvrma.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3qtlonkgm.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3dniyzyiy.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3qwsuprtf.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3dkoqamgw.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3vrgpgqgg.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3bsfhqmfn.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xwurtpdz.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3bfuxrjvu.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3aishwgbw.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3rgljtade.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3hvwkzmcf.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3vgxiznix.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3jrymbksy.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3emuuhetm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3pdkramrw.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3zhiuofis.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3dtfkrmod.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vnhdardk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3cfyxrdww.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3qlpluccb.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3kxzfjvgj.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3mdgfthah.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ezmquvjl.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3vhskozlm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3aweaycbt.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3lplsiegx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3bydmuwxk.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3mfoctsxw.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3ohroqlcp.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3waijpoft.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vyhynogv.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rwoirupn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3utrhmhqc.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3qnkytmbl.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3ulollyoz.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3cnbkxnue.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3duwreahp.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3cbprzbsp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3trgqhwnf.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3nynbeveo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3ccbjaeoz.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3fpovtglx.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3moftehxe.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3mfxsecug.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3ahaqixfi.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3ukcpwama.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3wkvnapkj.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3tgouacvi.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3foknjgsl.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3uddcytvm.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3hpemiclx.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3niogvxls.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3smkrtzcc.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3iqfwktao.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3vambucfv.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3yusjetmd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3emeyxjpu.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3urpaukjt.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3ysfckjxw.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3xeofoqol.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3oljanjpc.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pqhurhfy.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3guxyatuc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3egitvyxq.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3ecnpxikg.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3hbvmkyjy.html


<!-- 参考信息 -->