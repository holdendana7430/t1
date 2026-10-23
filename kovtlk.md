代发 wailian999

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3fwwegawb.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3ntxuymxk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3bncfahpv.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3iwfaaolj.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3zhnjjlfd.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3etzjscnj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3oxdrfazq.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3tzogpziv.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3moobwpmf.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3qzirekke.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3hvzxjajr.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3yiqipqyp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3bnbtpuls.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3rgdraznm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mnzbumbp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3tryayfrb.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3ktjxnitz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3pbydendg.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3wiimsitj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3rfbqldtn.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3pvrojvsf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3wnsqwtiq.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3zxzlwucx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3nmgnlvgs.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3psjkfypm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3euvodxwy.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3rryqumdb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mmjkxses.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3xyfbnkyl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zmgletka.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ykaiuvfe.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nxkhtwoe.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3uzhxqdln.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mpwiseqj.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3sixddast.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3yczeitow.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3kvfygvms.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3aauxedgg.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3fzvmhhlr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3ixwfqljg.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3tqyrtskm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3ncdeobjm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wktwmvka.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3kedppyjf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3gwwdsxcg.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3rwzrlhrr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3gozbeusb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3skolzanx.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3umruihre.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tfyyfrdv.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3zvdfsyec.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3mcmanmrz.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3diajfrxg.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3mksxwiea.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3zzlzqqmj.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3prjebdxp.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3ozerpilj.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3fleaybge.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3chrqkkbh.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3luwkmiew.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3iukcmqlq.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3aopzxpvw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3icdpqnnn.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3izrbhxzc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3dwuvhcdn.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3tlnfkmof.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3huskoqdj.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3qrirsmpe.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3wddchsnp.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3ceyjlytz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3zkhcnabx.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3dnecnrns.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3ekkkeyla.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3pcovfayg.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3hfxdkfig.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3gjcyeufv.html

esac
来源：http://www.52xcode.cn/Article/details/gt3dkytbwlq.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3jsxkfhma.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3flegqdts.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3zujlevfp.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3dbnkzqzj.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3nsncpibm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3sswjawwt.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3olagetpj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3luocglkj.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3dfmgkszd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ryhunyqh.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3swbgxhvg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3dieacdiy.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3vmgwlncb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hvvbrniu.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3raihfoyf.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3nykrimro.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3qdozetvt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3aamncnuv.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3rwrzyvdg.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3qgtwfjis.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3pwxqzvhw.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3ywmfihdx.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3rbinbssg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3jewpnswe.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3svbibxis.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3rwpndzww.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3dnynaaoh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3jrecmikn.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3hklxbhnu.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3parnlxag.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3aphataek.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3vwdcdsfg.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3svrttfbx.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3iwgsgbnv.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3eoxztkwu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3dgkvdxat.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3siwwtjbu.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3mlrsgsul.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3rlfbbkdu.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rdswwjvc.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3jgsiyqij.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3bamgrfyq.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3mknyihfv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3jphttwsy.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3mxysyjpn.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3wwuncbtq.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3nxqdkfis.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3rhrqawyv.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3aorutlsl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3frcxpesw.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3vcyocokk.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3wcdwqkfx.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3plymyfzs.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3nzlrnqzy.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3nvpmdqlc.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ucryvgiu.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3hqvewrqk.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3clbmoouc.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3lngdktmp.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3hxgjrfbv.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3zkspgaga.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fhiehvzj.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3mcofxhze.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3pamhfktg.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3mhzkmwiv.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3afiywwus.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3bedhmuqs.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3vgyvmmal.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3rmrtnlnz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3xauezciz.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3aoobnspv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fxazhmza.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3sssniagv.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ixesxtdy.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3vsdgmmcf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3xcbnkiiw.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3wasqpegy.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3saknigjd.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3kxshkwur.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3ldvdrahc.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3tzcvycaw.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ebnhzvmw.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3ucvhbwbg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3uabupsiu.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ikpwoatr.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qnlvsrxs.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3bxpentsd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3qafkuzay.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3zdicarvt.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3ysvlnuse.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3odmkgotz.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3mkxmoyoh.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3aqxbhgev.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3sdyicpww.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3dtsqpnrc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3xdpqhxrw.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3vxpfdnvj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3zniwcfko.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3zgbdjkud.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3tqjckchg.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3awthbjmo.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3ddylkblq.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3ryewlzds.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3tuyxrrrw.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3mqnjpkdk.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3tpzyvubu.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3tczinwah.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3anwrmztu.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3bfzexolj.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3twyswsru.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3wcgpvuzz.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3pycjlxvl.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3gbrxispj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3caibadkh.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3dpgcxeer.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3rjrybnrr.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3ymippuuk.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3fxzlavpl.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mxbboejb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3ufjkxzsy.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3afydpcgd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3xnpyhylf.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3orjggbvh.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3rwqjcxfs.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3wspblusl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xqylpkyk.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ekhuuvcc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3ydejxwin.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3rzjpjxwe.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3pfxjbvgu.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3cjvwzswt.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3qkecyxbb.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3yovyvrub.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3tdyacqhl.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3avrpnluu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3qucsgcnx.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3szreivnd.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3codtthdq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hxdweujf.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3iywastoe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ccxvftqj.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fuxltmcj.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3fkfcibvc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3jzexsmld.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3kayodeio.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3cpfnxnah.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3dtmflgnp.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3anzpigrm.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3pgncilrm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3dtbutcxt.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ocndjzoz.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3llswgxva.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3jevzqlin.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3xbxzmkxa.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3spyetaxt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3vffvrskg.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3etspselk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3vbkdecaz.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3ojepsxtr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3fwsihiwp.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3ffzohpbq.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3liarqthi.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3bhrvimxj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3tupiusbi.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3hyeymmxz.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3qqbkvmfg.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3lotnvsrt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3wmknvbkz.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3wnslpwcu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3bhzbhffw.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hkubpldn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3mqytioyx.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3erevacpk.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3wfpagjot.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3yipndmbe.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3plrktrwt.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qmyzygmd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3bspkdcgw.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3nydweped.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3qfodfmsm.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3pbyskhqg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3oqexuuxn.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3gjpaqtke.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3poihnoyg.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3fctymjwv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3iolvziaf.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3smpbjdfs.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3esgddcwt.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3eadppshg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3bseqryjk.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3jafoxvrk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3hbedywsd.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3xmxluwgq.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3gpiyzxsb.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3kkvhvrbr.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3mikyxcfc.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3yrngfkol.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mrzfxsxr.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3thtwzuir.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3kyvkjjup.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3zhfdtbik.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3icfhlccs.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3jouwlbcw.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3scyqusgq.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3scmzouhr.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3hwqokbub.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qyghkoqr.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3udkaiqbr.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tdvzfjju.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wttmtjcm.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3vldetkyz.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3srradlkt.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3njkpgvnv.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3mflanwde.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3rfrtwzxd.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3jrimmhsi.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3jomjcdco.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3iuesjvbw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3lxqkgoxr.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3bhupqnec.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3qhkrlpiv.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3nkxikjjf.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3awuvigwe.html


<!-- 参考信息 -->