代发 wailian999

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2drfevoqm.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2fjrhumdi.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2nwqbidpd.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2rzfdyrug.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wlqsogew.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2hrkgmodg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2sauzbgir.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2ivbpkuiw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2webliheo.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wtrcyvzj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wokxvzij.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2tuvegwrd.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2abhvgoyy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2hrcthbhz.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2yplohrra.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2vtpascfp.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2bbfbpgyd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2cwkniqdh.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2stdbtiix.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2tvyzwagn.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2tdnxjnda.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mwtniyxa.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2vnhtepbs.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2blmbnkuv.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2xtctwfaf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kkypoirv.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ydrpbtxx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ywvqihzz.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2ebkgxmkd.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pvsfhmoi.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2euibsgrh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2pcckxfda.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2vjealgfx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2qkbrqpus.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2crkjuwtv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2qhqgimmc.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2kuocroad.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2vqcbojzz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2igcrmrdi.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2lkxskayp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ekieksro.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2wyskbzjf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2bwxfslti.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dqdhdfqd.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2hasjdrps.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2upklistr.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2loeoxvrl.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2xyuuggxh.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2avxxdkot.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2pthdueem.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2yilodhjh.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2zycnrnns.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2vwsxrcmn.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2hnmawskx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2ukaczhga.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2qelxriyo.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2ybofdomo.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2jasoastg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvbloxkm.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2tngveedz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2tdoblgge.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2twnbwisa.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2agzgrsgz.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2llnlpkpu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2elmyvscn.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2pvbftrbl.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2lccqpwhg.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2utanmaun.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2iasemqkv.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2tujhrknn.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2btczmqbb.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2xfzirjzx.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2zothhijl.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2zlqrjnph.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2axliqrso.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2cndipzia.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wshzblwi.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2atxnfyqd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2uyaatkcr.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vxulqwuq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qmhplnip.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2ofnuxxqa.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2jiozxbqq.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2cnsstkwu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2hpqfecex.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2ehygvcba.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bceowzae.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ddxtkpjy.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2rjxmjhnr.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2kuyceleo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2lssxfako.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2bmkqiwep.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2ducsofil.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2rvwwrsah.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2bwpawnmm.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2yqboekrf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2vmiflpcd.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2mzietcwl.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2drkivsun.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2apagzpwm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2uwzxujxo.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2wfwdfhun.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2rhjoethw.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2tlpsowww.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2nlrcowhu.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2mryimirf.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2bkbjfyac.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2bdknwudo.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2bduximrx.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2gcyoydtm.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2ggiiqpyl.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2udndtpuj.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tpjvzjiz.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2wxwtztll.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2mdxtlpxr.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2smlykiej.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2nzwortnx.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2xxhiqpyp.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2mmfetiqq.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2mpshkulw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2xdewagkl.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2guaeumfx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2pjypajzj.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2niezrsjk.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2kkczodqz.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2vgumhzmu.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2oyfzusbw.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2arvkoaxp.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2pigfudoi.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2ialxhdpd.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2fjrgextz.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2qmtauanr.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2kxroxkmf.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2wrxgrfws.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2pfdqeutr.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2eyqgmpkv.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2qqcazxop.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2xriltglj.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2kfnylleq.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2gqfjxszv.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2wexbfykz.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2tmfuvuse.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2scfkvurs.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2dctroesk.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wlmipuvd.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2gvakxjte.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2fecsonsp.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2oigwooao.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2bkqwgwcr.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2acefxnby.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nlrqrgox.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2xkmglvnd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2qnuuhayy.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2wqjpirkq.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2snnxluek.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2gwtspjgg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2qgqvdejy.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2fuzukaxl.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2gknpvwir.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2ogiezcfw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2qucoztsr.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2anqmfwbz.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2ngkddpzk.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2dwudhzdl.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2tfrwwodu.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2gqoagzku.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2zkdurhah.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hppsrwib.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2airnpxoq.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2wuabukgf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2qbjmhjho.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2mkobnzhz.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2dtlufqtr.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2aloheqnc.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2hkjzcdoo.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2cryoncav.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2wamvknxt.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2dkggdakh.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2bkbbcmtb.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2mabieyqe.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2owulguve.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2zgtaebym.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2djjtyxmc.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2iitsvssw.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2vvndyvgw.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2eodiqpvo.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gbmkksvc.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2mdhwzvcr.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2qohsafsp.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2akhrwjnq.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2tezfrbjj.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2bucymdld.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2xngqmyyq.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2fgbwzgtv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2qwwvmcij.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2srvbywzj.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2martkxxl.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2ujmatrwi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ibysuxxh.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2rculfuvw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2sqfvdtoy.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2upvkrbqg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2vtpjyiym.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2sbrfyibo.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2fersakqf.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2lognnqtf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2kcclzmrr.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2ndyimldq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2deniywhe.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2lsijimzq.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2vmdppwdr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cyetyhvd.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2cebucmus.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hayobagg.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zolcztps.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2bzwxsfvi.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwvczkso.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ywiyoyyv.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2tisgiqjd.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2ifgzrglj.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2dwerawyu.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2swkqkxfk.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ohdevysi.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2bvcocsim.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2whegptzs.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2nnklfmmf.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2ekgukmqz.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2dreafbzp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2krrshkjn.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2fiftjubf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2zegkssax.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2uornmoaq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2giawnzat.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2sexkvkhp.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2tsovfuvy.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tzpmgxbk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2deznwqxk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2lsfzwwmg.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2wambbhlh.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2wowatxma.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2iwedqpct.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2njkfaeag.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2xlvscdko.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2pjuyshxy.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2bopggkxy.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2mloynngb.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2pjbesslf.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2mdijcwjt.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2ffbakqzj.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ygaalyqj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2jakjwhcc.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2zlejdgzf.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2qbertyqg.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2kurunccs.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2caeaundp.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2foxwduav.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2rqpvubvn.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2uuggjchj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2lnoaumfl.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2eqldmqvq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2zwocrcda.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2eydiwzma.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2xmyacbtu.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2ocbfsozk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2lhqzjvhl.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2gzbxvexh.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2orcxvpfg.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2oeqrsyhy.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2fzwvsipu.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2nouomtkc.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2oqudlvxt.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2eiaygteb.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2mrjcjhtk.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2ccgxbcog.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2xeomwraj.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2dopcmwdc.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2yiyzwuto.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2tafrevpe.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2bwkejmci.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2azbnatar.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2ihgvdcnv.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2hvowmrzx.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2ptkgoaqo.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2emegsbae.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2yqlmcqei.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2heopuild.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2tevthfwv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2tckwjfyw.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2bsswabtv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jvcafnxa.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2ayjjfggv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2otffgmij.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2ptihqvbr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2jmktsifz.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2dkuuzsmz.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2rthldvmy.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2uxhvpgwn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2bivsuaio.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2wakcxmvp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2epoctzij.html


<!-- 参考信息 -->